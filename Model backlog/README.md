## Model backlog (list of the developed model and it's score)
- **Train** and **validation** are the splits using the train data from the competition.
- The competition metric is **Quadratic Weighted Kappa**.
- **Pb Leaderboard** is the Public Leaderboard score.
- **Pv Leaderboard** is the Private Leaderboard score.

---

## Models

|Model|Train|Validation|Pb Leaderboard|Pv Leaderboard|
|-----|-----|----------|--------------|--------------|
|1 - ResNet50 - Batch size 8|???|???|???|???|
|2 - ResNet50 - Img 640x640|???|???|???|???|
|3 - ResNet50 - Img 768x768|???|???|???|???|
|4 - ResNet50 - Batch size 32|???|???|???|???|
|5 - ResNet50 - Img 779×779|???|???|???|???|
|6 - ResNet50 - Img 450×450|???|???|???|???|
|7 - ResNet50 - Threshold optimization|???|???|???|???|
|8 - ResNet50 - Class weights|???|???|???|???|
|9 - ResNet50 - Kappa metric|???|???|???|???|
|10 - ResNet50 - optimize Kappa|???|???|???|???|
|11 - ResNet50 - Vertical flip opt|???|???|???|???|
|12 - ResNet50 - Vertical flip norm|???|???|???|???|
|13 - ResNet50 - Threshold opt complete set|???|???|???|???|
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
