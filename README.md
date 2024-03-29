# DeepLab3 with ResNet Transfer Learning Pipeline for Lung Cancer Segmentation

## Introduction
* Model Used: DeepLabV3 https://arxiv.org/abs/1802.02611v3
* Feature Decoder: Pretrained ResNet50, ResNet101
* Fixed Hyperparameter: learning rate, activation function
* Tweerked Hyperparameter: optimizer, loss function
* Dataset: CT images from http://medicaldecathlon.com/

## Explaination
* Use DeepLabV3 with ResNet101 to perform the lung cancer segmentation
* Perform hyperparameter tuning for the model to find the best-performed hyperparameter
* Feature Decoder: Pretrained ResNet50, ResNet101
* Optimizer: Adam / SGD / Adagrad
* Loss Function: BCEwithlogits / DiceLoss / BinaryFocalLoss

## Result
* ResNet50 + SGD + DiceLoss have the best result of Dice Coefficient 0.803

![alt text](/api/asset/download?experimentKey=1587b6cfaf2a4fe69d94f684782c4a30&assetId=dcd116a70d484d14a3810452d5023436)
