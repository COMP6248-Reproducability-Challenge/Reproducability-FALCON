Reproducability-REFORMER
===
---

Origin paper:

REFORMER: THE EFFICIENT TRANSFORMER

https://openreview.net/forum?id=BylXi3NKvS



## Overview
#### Code structure
``` Unicode
FALCON
  │ 
  ├── src
  │    │     
  │    ├── models
  │    │     ├── vgg.py: VGG model
  │    │     ├── resnet.py: ResNet model
  │    │     ├── model_imagenet.py: Pretrained model (from pytorch) 
  │    │     ├── falcon.py: FALCON
  │    │     └── stconv_branch.py: StConvBranch & FALCONBranch
  │    │      
  │    ├── train_test
  │    │     ├── imagenet.py: train/validate on ImageNet 
  │    │     ├── main.py: train/test on CIFAR10/CIFAR100/SVHN 
  │    │     ├── train.py: training process
  │    │     ├── test.py: testing process
  │    │     └── validation.py: validation process
  │    │     
  │    └── utils
  │          ├── compression_cal.py: calculate the number of parameters and FLOPs
  │          ├── default_param.py: default cfgs 
  │          ├── load_data.py: load datasets
  │          ├── lr_decay.py: control learning rate
  │          ├── optimizer_option.py: choose optimizer 
  │          ├── save_restore.py: save and restore trained model
  │          └── timer.py: timer for inference time
  │
  └── script: shell scripts for execution of training/testing codes
```

## License
Licensed under the Apache License, Version 2.0
