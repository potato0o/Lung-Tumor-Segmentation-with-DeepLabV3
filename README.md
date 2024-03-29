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
* Dice Loss on Validation Dataset for ResNet50 + SGD + DiceLoss
![Dice Loss on Validation Dataset](https://github.com/potato0o/Lung-Tumor-Segmentation-with-DeepLabV3/blob/main/Result/ValDice.jpeg)
![Dice Loss on Validation Dataset](https://github.com/potato0o/Lung-Tumor-Segmentation-with-DeepLabV3/blob/main/Result/Val%20Prediction%20vs%20Label.jpeg)
