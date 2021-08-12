# textile-defect-detection
In the context of textile fabric, rare anomaly can occurs, hence compromizing the quality of the tissus. In order to avoid that in some scenario, it is crucial to detect the defect.

## Overview and Goal


## Model Architectures

* CNN
* ResNet18

## Results

| Models    | Accuracy | Train Loss | Validation Loss | Transformations |
|-----------|----------|------------|-----------------|-----------------|
| ResNet18  |          |            |                 |                 |
| ResNet34  |          |            |                 |                 |
| ResNet101 |          |            |                 |                 |

## Future Works


### Model Summaries

**ResNet18**
```
Classification Task: Keepíng all the data
----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1            [1, 64, 16, 16]           3,136
       BatchNorm2d-2            [1, 64, 16, 16]             128
              ReLU-3            [1, 64, 16, 16]               0
         MaxPool2d-4              [1, 64, 8, 8]               0
        Conv2dAuto-5              [1, 64, 8, 8]          36,864
       BatchNorm2d-6              [1, 64, 8, 8]             128
              ReLU-7              [1, 64, 8, 8]               0
        Conv2dAuto-8              [1, 64, 8, 8]          36,864
       BatchNorm2d-9              [1, 64, 8, 8]             128
 ResNetBasicBlock-10              [1, 64, 8, 8]               0
       Conv2dAuto-11              [1, 64, 8, 8]          36,864
      BatchNorm2d-12              [1, 64, 8, 8]             128
             ReLU-13              [1, 64, 8, 8]               0
       Conv2dAuto-14              [1, 64, 8, 8]          36,864
      BatchNorm2d-15              [1, 64, 8, 8]             128
 ResNetBasicBlock-16              [1, 64, 8, 8]               0
      ResNetLayer-17              [1, 64, 8, 8]               0
           Conv2d-18             [1, 128, 4, 4]           8,192
      BatchNorm2d-19             [1, 128, 4, 4]             256
       Conv2dAuto-20             [1, 128, 4, 4]          73,728
      BatchNorm2d-21             [1, 128, 4, 4]             256
             ReLU-22             [1, 128, 4, 4]               0
       Conv2dAuto-23             [1, 128, 4, 4]         147,456
      BatchNorm2d-24             [1, 128, 4, 4]             256
 ResNetBasicBlock-25             [1, 128, 4, 4]               0
       Conv2dAuto-26             [1, 128, 4, 4]         147,456
      BatchNorm2d-27             [1, 128, 4, 4]             256
             ReLU-28             [1, 128, 4, 4]               0
       Conv2dAuto-29             [1, 128, 4, 4]         147,456
      BatchNorm2d-30             [1, 128, 4, 4]             256
 ResNetBasicBlock-31             [1, 128, 4, 4]               0
      ResNetLayer-32             [1, 128, 4, 4]               0
           Conv2d-33             [1, 256, 2, 2]          32,768
      BatchNorm2d-34             [1, 256, 2, 2]             512
       Conv2dAuto-35             [1, 256, 2, 2]         294,912
      BatchNorm2d-36             [1, 256, 2, 2]             512
             ReLU-37             [1, 256, 2, 2]               0
       Conv2dAuto-38             [1, 256, 2, 2]         589,824
      BatchNorm2d-39             [1, 256, 2, 2]             512
 ResNetBasicBlock-40             [1, 256, 2, 2]               0
       Conv2dAuto-41             [1, 256, 2, 2]         589,824
      BatchNorm2d-42             [1, 256, 2, 2]             512
             ReLU-43             [1, 256, 2, 2]               0
       Conv2dAuto-44             [1, 256, 2, 2]         589,824
      BatchNorm2d-45             [1, 256, 2, 2]             512
 ResNetBasicBlock-46             [1, 256, 2, 2]               0
      ResNetLayer-47             [1, 256, 2, 2]               0
           Conv2d-48             [1, 512, 1, 1]         131,072
      BatchNorm2d-49             [1, 512, 1, 1]           1,024
       Conv2dAuto-50             [1, 512, 1, 1]       1,179,648
      BatchNorm2d-51             [1, 512, 1, 1]           1,024
             ReLU-52             [1, 512, 1, 1]               0
       Conv2dAuto-53             [1, 512, 1, 1]       2,359,296
      BatchNorm2d-54             [1, 512, 1, 1]           1,024
 ResNetBasicBlock-55             [1, 512, 1, 1]               0
       Conv2dAuto-56             [1, 512, 1, 1]       2,359,296
      BatchNorm2d-57             [1, 512, 1, 1]           1,024
             ReLU-58             [1, 512, 1, 1]               0
       Conv2dAuto-59             [1, 512, 1, 1]       2,359,296
      BatchNorm2d-60             [1, 512, 1, 1]           1,024
 ResNetBasicBlock-61             [1, 512, 1, 1]               0
      ResNetLayer-62             [1, 512, 1, 1]               0
    ResNetEncoder-63             [1, 512, 1, 1]               0
AdaptiveAvgPool2d-64             [1, 512, 1, 1]               0
           Linear-65                     [1, 6]           3,078
    ResnetDecoder-66                     [1, 6]               0
================================================================
Total params: 11,173,318
Trainable params: 11,173,318
Non-trainable params: 0
----------------------------------------------------------------
Input size (MB): 0.00
Forward/backward pass size (MB): 1.23
Params size (MB): 42.62
Estimated Total Size (MB): 43.86
----------------------------------------------------------------
Total_params 11173318
Trainable_params 11173318
```

Contributors: Emre Okcular, Hashneet Kaur