## Model backlog (list of the developed model and it's score)
- **Train** and **validation** are the splits using the train data from the competition.
- The competition metric is **Quadratic Weighted Kappa**.
- **Pb Leaderboard** is the Public Leaderboard score.
- **Pv Leaderboard** is the Private Leaderboard score.

---

## Models

|Model|Train|Validation|Pb Leaderboard|Pv Leaderboard|
|-----|-----|----------|--------------|--------------|
|1 - ResNet50 - Batch size 8|0.954|???|0.714|???|
|2 - ResNet50 - Img 640x640|0.934|???|0.660|???|
|3 - ResNet50 - Img 768x768|0.914|???|0.583|???|
|4 - ResNet50 - Batch size 32|0.917|???|0.553|???|
|5 - ResNet50 - Img 779×779|0.957|???|0.576|???|
|6 - ResNet50 - Img 450×450|0.935|???|0.701|???|
|7 - ResNet50 - Threshold optimization|0.937|0.896|0.755|???|
|8 - ResNet50 - Class weights|0.936|0.888|0.680|???|
|9 - ResNet50 - Kappa metric|0.954|0.906|0.674|???|
|10 - ResNet50 - optimize Kappa|0.988|0.908|0.567|???|
|11 - ResNet50 - Vertical flip opt|0.935|0.897|0.705|???|
|12 - ResNet50 - Vertical flip norm|0.935|0.909|0.647|???|
|13 - ResNet50 - Threshold opt complete set|0.932|0.882|0.735|???|
|14 - ResNet50 - Threshold opt validation set|0.927|0.890|0.615|???|
|15 - ResNet50 - 224x224|0.927|0.881|0.704|???|
|16 - ResNet50 - Stratified split|0.916|0.878|0.572|???|
|17 - ResNet50 - Rotation range|0.939|0.915|0.659|???|
|18 - ResNet50 - Zoom range|0.956|0.912|0.428|???|
|19 - ResNet50 - Brightness range|0.968|0.888|0.595|???|
|20 - ResNet50 - Brightness range|0.952|0.895|0.555|???|
|21 - ResNet50 - Zoom range 0.2|0.947|0.892|0.580|???|
|22 - ResNet50 - Zoom range fill constant|0.935|0.895|0.704|???|
|23 - ResNet50 - Data augmentation fill constant|0.930|0.906|0.707|???|
|24 - ResNet50 - Data augmentation fill reflect|0.939|0.920|0.688|???|
|25 - ResNet50 - Img 224x224|0.944|0.896|0.616|???|
|26 - ResNet50 - Img 256x256|0.930|0.866|0.693|???|
|27 - ResNet50 - Img 224x224 batch 64|0.899|0.867|0.699|???|
|28 - ResNet50 - Train augmentation only|0.902|0.874|0.647|???|
|29 - ResNet50 - Train augment, Validation thr opt|0.897|0.872|0.599|???|
|30 - ResNet50 - Train augment, 256x256|0.917|0.890|0.664|???|
|31 - ResNet50 - SGD optimizer, 2 steps|0.904|0.879|0.676|???|
|32 - ResNet50 - SGD optimizer, 1 step|0.920|0.897|0.699|???|
|33 - ResNet50 - Step decay|0.932|0.877|0.673|???|
|34 - ResNet50 - Cycle LR|0.853|0.857|0.606|???|
|35 - ResNet50 - Warmup 1 epoch|0.923|0.891|0.647|???|
|36 - ResNet50 - Warmup 3 epochs|0.936|0.906|0.701|???|
|37 - ResNet50 - Validation size 0.2|0.922|0.897|0.682|???|
|38 - ResNet50 - Validation size 0.15|0.947|0.917|0.674|???|
|39 - ResNet50 - 2 step fine-tuning|0.933|0.899|0.695|???|
|40 - ResNet50 - Class distribution threshold opt|0.909|0.904|0.705|???|
|41 - ResNet50 - Focal loss|0.912|0.892|0.743|???|
|42 - ResNet50 - Cycle LR longer epochs|0.907|0.863|0.652|???|
|43 - ResNet50 - Cycle LR epochs 40|0.926|0.891|0.647|???|
|44 - ResNet50 - Cycle LR and Focal loss|0.888|0.864|0.689|???|
|45 - ResNet50 - Focal loss - 320x320|0.922|0.889|0.658|???|
|46 - ResNet50 - Focal loss - Simple augmentation|0.956|0.885|0.716|???|
|47 - ResNet50 - Focal loss - CV2 resize|0.938|0.878|0.694|???|
|48 - ResNet50 - Focal loss - Crop relevant areas|0.926|0.90|0.720|???|
|49 - ResNet50 - Focal loss - TTA|0.934|0.899|0.701|???|
|50 - ResNet50 - Batch size 8|0.944|0.902|0.724|???|
|51 - ResNet50 - Threshold opt complete set|0.945|0.907|0.723|???|
|52 - ResNet50 - Gray scale|0.933|0.906|0.740|???|
|53 - ResNet50 - RGB scale|0.967|0.893|0.708|???|
|54 - ResNet50 - Gray circular cropping|0.935|0.846|0.726|???|
|55 - ResNet50 - RGB circular cropping|0.948|0.890|0.692|???|
|56 - ResNet50 - Gray Ben's Preprocessing|0.919|0.866|0.711|???|
|57 - ResNet50 - RGB Ben's Preprocessing|0.945|0.884|0.754|???|
|58 - ResNet50 - Gray Ben's process, circular crop|0.880|0.849|0.712|???|
|59 - ResNet50 - RGB Ben's process, circular crop|0.960|0.860|0.699|???|
|60 - ResNet50 - Gray, circular crop sigma 30|0.889|0.851|0.678|???|
|61 - ResNet50 - RGB, circular crop sigma 30|0.929|0.894|0.656|???|
|62 - ResNet50 - Regression - Gray scale|0.928|0.867|0.718|???|
|63 - ResNet50 - Regression - RGB scale|0.949|0.901|0.719|???|
|64 - ResNet50 - Regression - Gray Zoom range|0.899|0.853|0.687|???|
|65 - ResNet50 - Regression - RGB Zoom range|0.916|0.886|0.693|???|
|66 - ResNet50 - Regression - Warmup 5 epochs|0.927|0.900|0.721|???|
|67 - ResNet50 - Regression - Lower earlystopping|0.915|0.892|0.687|???|
|68 - ResNet50 - Regression - Batch size 32|0.933|0.888|0.703|???|
|69 - ResNet50 - Regression - Image size 224|0.937|0.891|0.704|???|
|70 - ResNet50 - Regression - 1 generator|0.927|0.872|0.699|???|
|71 - ResNet50 - Regression - Finu-tune top|0.000|0.000|000|???|
|72 - ResNet50 - Regression - Finetune top 1st conv|0.000|0.000|000|???|
|73 - ResNet50 - Regression - Finetune top |0.000|0.000|000|???|
|74 - ResNet50 - Regression - Incresing batch size|0.949|0.880|0.660|???|
|75 - ResNet50 - Regression - Increasing img size|0.922|0.878|0.651|???|
|76 - ResNet50 - Regression - TTA 5|0.938|0.880|0.696|???|
|77 - ResNet50 - Regression - Imgaug generator|0.966|0.883|0.699|???|
|78 - ResNet50 - Regression - TTA 8|0.924|0.885|0.709|???|
|79 - ResNet50 - Regression - Albumentations|0.962|0.883|0.701|???|
|80 - ResNet50 - Regression - Imgaug clean|0.970|0.869|0.700|???|
|81 - ResNet50 - Regression - Keras aug Crop v2|0.944|0.894|0.731|???|
|82 - ResNet50 - Regression - Imgaug Crop v2|0.963|0.884|0.731|???|
|83 - ResNet50 - Regression - Albumentation Crop v2|0.965|0.893|0.719|???|
|84 - VGG16 - Regression|0.794|0.767|0.619|???|
|85 - VGG19 - Regression|0.736|0.693|0.577|???|
|86 - Xception - Regression|0.951|0.889|0.746|???|
|87 - InceptionResNetV2 - Regression|0.957|0.891|0.742|???|
|88 - InceptionV3 - Regression|0.922|0.888|0.736|???|
|89 - MobileNet 128 - Regression|0.899|0.863|0.692|???|
|90 - MobileNet 224 - Regression|0.893|0.864|0.694|???|
|91 - NASNetMobile - Regression|0.913|0.889|0.740|???|
|92 - NASNetLarge - Regression|0.969|0.879|0.761|???|
|93 - MobileNetV2 - Regression|0.910|0.873|0.701|???|
