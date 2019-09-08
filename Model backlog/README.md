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
|94 - DenseNet121 - Regression|0.924|0.875|0.740|???|
|95 - DenseNet169 - Regression|0.935|0.878|0.757|???|
|96 - DenseNet201 - Regression|0.959|0.902|0.738|???|
|97 - ResNet50 - Regression - Default size|0.925|0.863|0.710|???|
|98 - VGG16 - Regression - Default size|0.734|0.699|0.619|???|
|99 - VGG19 - Regression - Default size|0.808|0.780|0.658|???|
|100 - Xception - Regression - Default size|0.955|0.887|0.732|???|
|101 - InceptionResNetV2 - Regression - Default size|0.953|0.877|0.739|???|
|102 - InceptionV3 - Regression - Default size|0.980|0.899|0.744|???|
|103 - NASNetMobile - Regression - Default size|0.900|0.887|0.718|???|
|104 - NASNetLarge - Regression - Default size|0.948|0.897|0.757|???|
|105 - MobileNet 128 - Regression - Default size|0.847|0.805|0.583|???|
|106 - MobileNet 224 - Regression - Default size|0.886|0.853|0.670|???|
|107 - MobileNetV2 - Regression - Default size|0.839|0.799|0.717|???|
|108 - DenseNet121 - Regression - Default size|0.916|0.864|0.704|???|
|109 - DenseNet169 - Regression - Default size|0.939|0.870|0.743|???|
|110 - DenseNet201 - Regression - Default size|0.928|0.883|0.737|???|
|111 - EfficientNetB0 - Regression|0.946|0.876|0.732|???|
|112 - EfficientNetB1 - Regression|0.950|0.889|0.732|???|
|113 - EfficientNetB2 - Regression|0.955|0.895|0.737|???|
|114 - EfficientNetB3 - Regression|0.958|0.898|0.743|???|
|115 - EfficientNetB4 - Regression|0.940|0.889|0.744|???|
|116 - EfficientNetB5 - Regression|0.961|0.907|0.746|???|
|117 - EfficientNetB0 - Regression - Default size|0.941|0.880|0.723|???|
|118 - EfficientNetB1 - Regression - Default size|0.940|0.880|0.721|???|
|119 - EfficientNetB2 - Regression - Default size|0.951|0.895|0.737|???|
|120 - EfficientNetB3 - Regression - Default size|0.947|0.891|0.734|???|
|121 - EfficientNetB4 - Regression - Default size|0.964|0.903|0.751|???|
|122 - EfficientNetB5 - Regression - Default size|0.956|0.894|0.756|???|
|123 - NASNetLarge - Classification|0.950|0.877|0.746|???|
|124 - DenseNet169 - Classification|0.928|0.892|0.757|???|
|125 - DenseNet169 - Classification - Default size|0.949|0.898|0.751|???|
|126 - NASNetLarge - Classification - Default size|0.944|0.894|0.751|???|
|127 - EfficientNetB5 - Classification|0.944|0.905|0.753|???|
|128 - EfficientNetB5 - Classification - Default size|0.936|0.901|0.749|???|
|129 - EfficientNetB5 - Classification - Attention|0.981|0.891|0.741|???|
|130 - EfficientNetB5 - Regression - Attention|0.961|0.894|0.736|???|
|131 - DenseNet169 - Classification - Attention|0.939|0.884|0.747|???|
|132 - NASNetLarge - Regression - Attentention|0.937|0.883|0.737|???|
|133 - DenseNet169 - Classification - Refactor|0.962|0.900|0.735|???|
|134 - DenseNet169 - Regression - Refactor|0.931|0.867|0.724|???|
|135 - EfficientNetB5 - Classification - Refactor|0.946|0.901|0.733|???|
|136 - NASNetLarge - Regression - Dft size - Refactor|0.976|0.902|0.732|???|
|137 - EfficientNetB5 - Regression - Dft size - Ref|0.963|0.904|0.737|???|
|138 - NASNetLarge - Regression - Refactor|0.931|0.880|0.741|???|
|139 - NASNetLarge - Regression - TTAx10|0.939|0.893|0.745|???|
|140 - EfficientNetB5 - Regression - TTAx10|0.958|0.900|0.759|???|
|141 - EfficientNetB5 - Regression - 2step finetune|0.951|0.895|0.746|???|
|142 - EfficientNetB5 - Regression - LR warmup|0.956|0.905|0.755|???|
|143 - EfficientNetB5 - Reg - Cosine LR decay|0.951|0.913|0.756|???|
|144 - EfficientNetB5 - Reg - Cosine LR decay Plt 3|0.944|0.909|0.771|???|
|145 - EfficientNetB5 - Reg - LR warmup, RMSprop|0.976|0.908|0.755|???|
|146 - EfficientNetB5 - Reg - Cosine LR, RMSprop|0.951|0.914|0.771|???|
|147 - EfficientNetB5 - Reg- Cosine LR Plt, RMSprop|0.950|0.906|0.755|???|
|148 - EfficientNetB5 - Reg- Zoom augmentation 125%|0.969|0.913|0.745|???|
|149 - EfficientNetB5 - Reg- Cyclical LR triangular|0.966|0.921|0.740|???|
|150 - EfficientNetB5 -Reg- Cyclical LR triangular2|0.950|0.908|0.761|???|
|151 - EfficientNetB5 -Reg- Cyclical LR exp_range|0.944|0.911|0.738|???|
|152 - EfficientNetB5 -Class-Cycl LR Lbl Smoothig01|0.966|0.910|0.726|???|
|153 - EfficientNetB5 -Reg- Cyc LR triangular2 Adam|0.936|0.900|0.765|???|
|154 - EfficientNetB5 -Reg- Cyc LR triangular2 Zoom|0.941|0.902|0.755|???|
|155 - EfficientNetB5 -Class- Cycl LR triangular2|0.962|0.898|0.744|???|
|156 - EfficientNetB5 -Class-Cycl LR Lbl Smoothig02|0.964|0.900|0.745|???|
|157 - EfficientNetB5 -Class-Cycl LR Lbl Smoothig03|0.972|0.904|0.753|???|
|158 - EfficientNetB5 - Classification - Focal loss|0.948|0.892|0.740|???|
|159 - EfficientNetB5 - Reg - Cosine LR, RMSprop2|0.931|0.888|0.755|???|
|160 - EfficientNetB5 - Reg - Zoom only on train|0.956|0.901|0.759|???|
|161 - EfficientNetB5 - Reg - Clean classifier|0.966|0.912|0.770|???|
|162 - EfficientNetB5 - Reg - Clean classifier2|0.965|0.908|0.769|???|
|163 - EfficientNetB5 - Reg - Batch 32, Img 224|0.962|0.895|0.769|???|
|164 - EfficientNetB0 - Reg - Batch 128, Img 224|0.982|0.893|0.726|???|
|165 - EfficientNetB5 - Reg - Adam Accumulate 4|0.937|0.899|0.725|???|
|166 - EfficientNetB5 - Reg - Adam Accumulate 8|0.931|0.897|0.712|???|
|167 - EfficientNetB5 - Reg - Big Classifier Concat|0.917|0.880|0.731|???|
|168 - EfficientNetB5 - Reg - Big Classifier Avg|0.953|0.909|0.742|???|
|169 - EfficientNetB5 - Reg - Big Classifier Max|0.960|0.902|0.768|???|
|170 - EfficientNetB5 - Reg - Cosine RAdam opt|0.981|0.895|0.752|???|
|171 - EfficientNetB5 - Reg - RAdam optimzer|0.956|0.897|0.751|???|
|172 - EfficientNetB3 - Reg - Batch 32, Img 224|0.977|0.889|0.731|???|
|173 - EfficientNetB5 - Reg - No Ben process|0.989|0.891|0.729|???|
|174 - EfficientNetB5 - Reg - Dropout|0.973|0.900|0.727|???|
|175 - EfficientNetB5 - Reg - No circle crop|0.977|0.901|0.754|???|
|176 - EfficientNetB5 - Reg - No Ben & Circle crop|0.966|0.885|0.702|???|
|177 - EfficientNetB5 - Reg - No crop|0.977|0.912|0.731|???|
|178 - EfficientNetB5 - Reg - RAdam optimizer|0.975|0.890|0.736|???|
|179 - EfficientNetB5 - Reg - Batch 32 Img 224 Plt2|0.974|0.897|0.751|???|
|180 - EfficientNetB5 - Reg - RAdam opt, Cosine|0.960|0.912|0.764|???|
|181 - EfficientNetB5 - Reg - RAdam opt|0.961|0.911|0.759|???|
|182 - EfficientNetB5 - Reg - Fold1 - Bs32, Img224|0.937|0.897|0.745|???|
|183 - EfficientNetB5 - Reg - Fold2 - Bs32, Img224|0.942|0.897|0.749|???|
|184 - EfficientNetB5 - Reg - Fold3 - Bs32, Img224|0.976|0.907|0.748|???|
|185 - EfficientNetB5 - Reg - Fold4 - Bs32, Img224|0.976|0.919|0.696|???|
|186 - EfficientNetB5 - Reg - Fold5 - Bs32, Img224|0.963|0.883|0.751|???|
|187 - EfficientNetB5 - Reg - 5-Fold Ensemble-Img224|0.962|0.963|0.766|???|
|188 - EfficientNetB5 - Reg - Fold1 - Img 456|0.951|0.907|0.742|???|
|189 - EfficientNetB5 - Reg - Fold2 - Img 456|0.972|0.909|0.738|???|
|190 - EfficientNetB5 - Reg - Fold3 - Img 456|0.940|0.921|0.730|???|
|191 - EfficientNetB5 - Reg - Fold4 - Img 456|0.948|0.920|0.739|???|
|192 - EfficientNetB5 - Reg - Fold5 - Img 456|0.962|0.904|0.743|???|
|193 - EfficientNetB5 -Reg- 5-Fold Ensemble-Img456|0.959|0.960|000|???|
|194 - EfficientNetB5-Reg-Old Data-Batch32 Img224|0.746|0.810|0.584|???|
|195 - EfficientNetB3-Reg-Old Data-Batch32 Img224|0.751|0.857|0.629|???|
|196 - EfficientNetB0-Reg-Old Data-Batch32 Img224|0.790|0.821|0.643|???|
|197 - EfficientNetB5 -Reg- 5-Fold-Img456 Inference|???|???|0.759|???|
|198 - EfficientNetB0-Reg-Old&New-Batch32 Img224|0.898|0.900|0.755|???|
|199 - EfficientNetB3-Reg-Old&New-Batch32 Img224|0.903|0.900|0.758|???|
|200 - EfficientNetB5-Reg-Old&New-Batch32 Img224|0.900|0.908|0.681|???|
|201 - EfficientNetB5-Reg-Old&New-Batch32 Img224 5e|0.907|0.906|0.766|???|
|202 - EfficientNetB5-Reg-Img224 0,5New data|0.927|0.907|0.771|???|
|203 - EfficientNetB5-Reg-Img224 0,3New data|0.802|0.908|0.772|???|
|204 - EfficientNetB3-Reg-Img224 0,5New data|0.849|0.898|0.769|???|
|205 - EfficientNetB5-Reg-Img224 0,5New data|0.908|0.899|0.771|???|
|206 - EfficientNetB5-Reg-Img224 0,5data No Ben|0.904|0.916|0.796|???|
|207 - EfficientNetB3-Reg-Img224 0,5data No Ben|0.909|0.911|0.791|???|
|208 - EfficientNetB5-Reg-Img224 0,5data Orig top|0.887|0.903|0.763|???|
|209 - EfficientNetB3-Reg-Img224 0,5data Orig top|0.894|0.902|0.762|???|
|210 - EffNetB5-Reg-Img224 0,5 Orig top No Ben|0.829|0.907|0.794|???|
|211 - EffNetB3-Reg-Img224 0,5 Orig top No Ben|0.896|0.912|0.785|???|
|212 - EfficientNetB5-Reg-Img224 0,3data No Ben|0.903|0.912|0.787|???|
|213 - EfficientNetB3-Reg-Img224 0,3data No Ben|0.908|0.908|0.791|???|
|214 - EfficientNetB5-Reg-Img224 0,5data No Ben 25e|0.767|0.906|0.775|???|
|215 - EfficientNetB3-Reg-Img224 0,5data No Ben 25e|0.918|0.916|0.788|???|
|216 - EfficientNetB5-Reg-Img456 0,5data No ben|0.875|0.917|0.707|???|
|217 - EfficientNetB5-Reg-Img224 0,5data Reg crop|0.903|0.911|0.785|???|
|218 - EfficientNetB5-Reg-Img256 0,5data No ben|0.901|0.910|0.780|???|
|219 - EfficientNetB4-Reg-Img256 0,5data No ben|0.919|0.912|0.783|???|
|220 - EfficientNetB4-Reg-Img256 0,5data LR1e-3/2|0.832|0.912|0.794|???|
|221 - EfficientNetB5-Reg-Img328 0,5data No ben|0.917|0.918|0.784|???|
|222 - EfficientNetB4-Reg-Img380 0,5data No ben|0.928|0.919|0.768|???|
|223 - EfficientNetB3-Reg-Img300 0,5data No ben|0.925|0.911|0.759|???|
|224 - EfficientNetB5-Reg-Img224 Old data|???|???|???|???|
|225 - EfficientNetB5-Reg-Img224 0,5data TTA 10|0.906|0.912|0.785|???|
|226 - EfficientNetB5-Reg-Img224 0,5data No TTA|0.847|0.910|0.777|???|
|227 - EfficientNetB5-Class-Img224 0,5data No Ben|0.702|0.868|000|???|
|228 - EfficientNetB5-Class-Img224 0,5 Focal Loss|0.709|0.874|000|???|
|229 - EfficientNetB5-Reg-Img224 0,5 Longer ES|0.932|0.911|0.789|???|
|230 - EfficientNetB5-Reg-Img224 0,5 Aug Flip|0.940|0.902|0.766|???|
|231 - EfficientNetB5-Reg-Img224 0,5 Aug Zoom|0.887|0.912|0.782|???|
|232 - EfficientNetB5-Reg-Img224 0,5 RAdam|0.912|0.905|0.791|???|
|233 - EfficientNetB5-Reg-Img224 0,5data Fold1|0.909|0.921|0.782|???|
|234 - EfficientNetB5-Reg-Img224 0,5data Fold2|0.823|0.898|000|???|
|235 - EfficientNetB5-Reg-Img224 0,5data Fold3|0.906|0.925|000|???|
|236 - EfficientNetB5-Reg-Img224 0,5data Fold4|0.895|0.923|000|???|
|237 - EfficientNetB5-Reg-Img224 0,5data Fold5|0.904|0.901|000|???|
|238 - EfficientNetB5-Reg-Img224 Old Pretrain NoBen|0.962|0.914|0.778|???|
|239 - EfficientNetB5-Reg-Img224 Old Pretrain|0.938|0.894|000|???|
|240 - EfficientNetB543 -Reg- 5-Fold Ensemble|0.949|0.923|0.795|???|
|241 - EfficientNetB5-Reg-Img456 Old Pretrain|0.955|0.904|0.773|???|
|242 - EfficientNetB5-Reg-Img328 Old Pretrain|0.964|0.909|000|???|
|243 - EfficientNetB5-Reg-Img256 Old Pretrain|0.964|0.903|0.791|???|
|244 - EfficientNetB5-Reg-Img224 Old Pretrain 10ep|0.965|0.911|0.773|???|
|245 - EfficientNetB5-Reg-Img224 Old&New Pretrained|0.944|0.908|0.785|???|
|246 - EfficientNetB5-Reg-Img256 Old&New Pretrained|0.939|0.910|0.791|???|
|247 - EfficientNetB5-Reg-Img328 Old&New Pretrained|0.940|0.908|0.790|???|
|248 - EfficientNetB5-Reg-Img224 Old data Balanced|???|???|???|???|
|249 - EfficientNetB5 -Reg- 5-Fold Img224 Old&New|0.959|0.963|0.803|???|
|250 - EffNetB5-Reg-224 Old Pretrain Balanced NoBen|0.941|0.907|0.770|???|
|251 - EffNetB5-Reg-224 Old Pretrain Balanced|0.924|0.892|000|???|
|252 - EffNetB5-Reg-256 Old Pretrain Balanced NoBen|0.925|0.894|000|???|
|253 - EffNetB5-Reg-328 Old Pretrain Balanced NoBen|0.936|0.908|000|???|
|254 - EffNetB5-Reg-224 0,3Old&New Balanced No Ben|0.931|0.911|0.768|???|
|255 - EffNetB5-Reg-Img224 Old Pretrain Sample STDV|0.967|0.913|0.786|???|
|256 - EffNetB5-Reg-Img224 Old Pretrain FeatureSTDV|0.944|0.902|000|???|
|257 - EffNetB5 -Reg- 5-Fold Img224 Old&New No Aug|0.957|0.959|0.796|???|
|258 - EffNetB5 -Reg- 5-Fold Img224 Old&New TTA 10|0.959|0.963|0.802|???|
|259 - EfficientNetB5-Reg-Img224 Balanced Fold1|0.932|0.920|000|???|
|260 - EfficientNetB5-Reg-Img224 Balanced Fold2|0.879|0.924|000|???|
|261 - EfficientNetB5-Reg-Img224 Balanced Fold3|0.907|0.917|000|???|
|262 - EfficientNetB5-Reg-Img224 Balanced Fold4|0.888|0.928|000|???|
|263 - EfficientNetB5-Reg-Img224 Balanced Fold5|0.811|0.887|000|???|
|264 - EffNetB5 -Reg- Img224 Old&New Resize ensemble|0.946|0.912|0.781|???|
|265 - EfficientNetB5-Reg-Img328 Old Pretrain Fold1|0.964|0.915|000|???|
|266 - EfficientNetB5-Reg-Img328 Old Pretrain Fold2|0.934|0.908|000|???|
|267 - EfficientNetB5-Reg-Img328 Old Pretrain Fold3|0.962|0.915|000|???|
|268 - EfficientNetB5-Reg-Img328 Old Pretrain Fold4|0.963|0.924|000|???|
|269 - EfficientNetB5-Reg-Img328 Old Pretrain Fold5|0.967|0.910|000|???|
|270 - EffNetB5 -Reg- 5-Fold 328 OldPretrain TTA 5|0.961|0.960|0.796|???|
|271 - EffNetB5 -Reg- 5-Fold 224 Balanced TTA 5|0.956|0.958|0.803|???|
|272 - EfficientNetB4-Reg-Img256 Old&New Fold1|0.697|0.877|000|???|
|273 - EfficientNetB4-Reg-Img256 Old&New Fold2|0.839|0.923|000|???|
|274 - EfficientNetB4-Reg-Img256 Old&New Fold3|0.738|0.899|000|???|
|275 - EfficientNetB4-Reg-Img256 Old&New Fold4|0.672|0.894|000|???|
|276 - EfficientNetB4-Reg-Img256 Old&New Fold5|???|???|???|???|
|277 - EffNetB5 -Reg- 5-Foldx2 Img224 TTA 5|0.959|0.960|0.804|???|
|278 - EfficientNetB4-Reg-Img224 Old data Balanced|0.800|0.716|000|???|
|279 - EfficientNetB4-Reg-Img256 Old Pretrain Fold1|0.929|0.902|000|???|
|280 - EfficientNetB4-Reg-Img256 Old Pretrain Fold2|0.933|0.895|000|???|
|281 - EfficientNetB4-Reg-Img256 Old Pretrain Fold3|0.965|0.921|000|???|
|282 - EfficientNetB4-Reg-Img256 Old Pretrain Fold4|0.964|0.920|000|???|
|283 - EfficientNetB4-Reg-Img256 Old Pretrain Fold5|0.965|0.898|000|???|
|284 - EfficientNet -Reg- 5-Fold Top5 TTA 5|0.951|0.921|000|???|
|285 - EffNetB5 -Reg- 5-Fold 224 Balanced TTA 5|0.948|0.947|0.780|???|
