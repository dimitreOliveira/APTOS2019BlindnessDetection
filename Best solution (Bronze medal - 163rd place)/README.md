# Solution overview

- **Data:**
  - Old data sampled to reduce samples from class 0.
  - Training set: Old data sampled and 4 folds of new data (80%).
  - Validation set: The other fold of new data (20%).
- **Model:** EfficientNetB5 (5-Fold).
- **Training:**
  - Warm-up classifier head (5 epochs).
  - Trained complete model (20 epochs).
- **Preprocess:**
  - Convert image to RGB channels.
  - Circle crop image.
  - Resize image to 224x224.
- **Augmentation:**
  - Rescale (divide by 255).
  - Random rotation 360°.
  - Random flip (horizontal and vertical).
- **Inference:** TTA x 10 and averaged all 5 models.


# Detailed solution

The problem was treated as a regression, this way should be easier to maximize the competition metric "Quadratic weighted Kappa", and also the labels had a semantic relationship between its neighbors, I Have also tried regular multiclass classification the results were worse. The loss function was "mean_squared_error" and the models' output were regular "linear" activation function.

- **[Data](https://github.com/dimitreOliveira/APTOS2019BlindnessDetection/blob/master/Best%20solution%20(Bronze%20medal%20-%20163rd%20place)/Train%20%26%20Validation%20split%20-%20(Old%2BNew).ipynb):**
  - Old data was sampled to a more balanced distribution, was used only 25% of samples from class 0.
  - Each fold had all sampled old data and 20% of new data.
  - Training set: All sampled old data and 80% of new data (15770 samples from old data and 2929 samples from new data).
  - Validation set: 20% of new data (733 samples).
![](https://raw.githubusercontent.com/dimitreOliveira/APTOS2019BlindnessDetection/master/Assets/fold_distribution.png)
- **Model:** EfficientNetB5
  - Imagenet pre-trained weights.
  - Replaced top head with GlobalAveragePooling2D and a Dense layer as linear output.
- **[Training](https://github.com/dimitreOliveira/APTOS2019BlindnessDetection/blob/master/Best%20solution%20(Bronze%20medal%20-%20163rd%20place)/233%20-%20EfficientNetB5-Reg-Img224%200%2C5data%20Fold1.ipynb):**
  - Parameters:
    - Batch size: 32
  - Warm-up step:
    - Freeze all layers except the last 2.
    - Learning rate: 4e-3, Adam optimizer and Cosine & Warm-up learning rate scheduler (2 epochs warm-up and hold base LR for 2 epochs).
    - Train for 5 epochs.
  - Fine-tunning step:
    - Unfreeze all layers.
    - Early stopping monitoring validation loss for 5 epochs.
    - Learning rate: 4e-4, Adam optimizer and Cosine & Warm-up learning rate scheduler (5 epochs warm-up and hold base LR for 3 epochs).
    - Train for 20 epochs.
#### Training learning rate policy scheduler (1 Fold):
![](https://raw.githubusercontent.com/dimitreOliveira/APTOS2019BlindnessDetection/master/Assets/fold_LR.png)
#### Training metrics (1 Fold):
![](https://raw.githubusercontent.com/dimitreOliveira/APTOS2019BlindnessDetection/master/Assets/fold_metrics.png)
![](https://raw.githubusercontent.com/dimitreOliveira/APTOS2019BlindnessDetection/master/Assets/fold_cf_matrix.png)
#### Test prediction distribution (1 Fold):
![](https://raw.githubusercontent.com/dimitreOliveira/APTOS2019BlindnessDetection/master/Assets/fold_pred_distribution.png)
- **Preprocess:** This step was applied before modeling to make training faster.
  - Convert image to RGB channels.
  - Circle crop image. This crop was used to remove black areas from original square images, and also crop a circular area based on the image center.
  - Resize image to 224x224. The original images size were reduced to 224, I have tried many others but this worked best, also made possible to train with larger batch size (32).
- **Augmentation:** All augmentations were from Keras ImageDataGenerator.
  - Rescale (divide by 255).
  - Random rotation 360°.
  - Random flip (horizontal and vertical).
- **[Inference](https://github.com/dimitreOliveira/APTOS2019BlindnessDetection/blob/master/Best%20solution%20(Bronze%20medal%20-%20163rd%20place)/258%20-%20EffNetB5%20-Reg-%205-Fold%20Img224%20Old%26New%20TTA%2010.ipynb):**
  - Test time augmentation (TTA) x10, using the same augmentations of the training step.
  - Averaged all the 5 models and their TTA predictions.
  - Threshold: [0.5, 1.5, 2.5, 3.5]
#### Inference metrics (5 Fold):
![](https://raw.githubusercontent.com/dimitreOliveira/APTOS2019BlindnessDetection/master/Assets/inference_cf_matrix.png)
#### Test prediction distribution (5 Fold, TTAx10):
![](https://raw.githubusercontent.com/dimitreOliveira/APTOS2019BlindnessDetection/master/Assets/inference_pred_distribution.png)
