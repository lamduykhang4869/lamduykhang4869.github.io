---
layout: post
title: Self-study Pytorch
subtitle: https://github.com/yunjey/pytorch-tutorial
cover-img: /assets/img/pytorch_logo_2018.svg
thumbnail-img: /assets/img/pytorch.png
share-img: /assets/img/pytorch_logo_2018.svg
tags: [pytorch]
---

## Pytorch basics

### Import Pytorch and Numpy library
import torch  
import torchvision  
import torch.nn as nn  
import torchvision.transforms as transforms  
import numpy as np  

### Create tensors 
x = torch.tensor(1., requires_grad=True)
