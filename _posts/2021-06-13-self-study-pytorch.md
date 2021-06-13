---
layout: post
title: Self-study Pytorch
subtitle: https://github.com/yunjey/pytorch-tutorial
cover-img: /assets/img/path.jpg
thumbnail-img: /assets/img/pytorch.png
share-img: /assets/img/path.jpg
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
_Create a tensor x with initial value is 1.0 (float) and record autograd._  
x = torch.tensor(1., requires_grad=True)   
w = torch.tensor(2., 
requires_grad=True)  
b = torch.tensor(3., required_grad=True)  

### Build a computational graph.
_y = 2 * x + 3_    
y = w * x + b 

