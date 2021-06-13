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
_Create a tensor x with initial value is 4.0 (float) and record autograd._  
x = torch.tensor(4., requires_grad=True)   
w = torch.tensor(2., 
requires_grad=True)  
b = torch.tensor(3., required_grad=True)  

### Build a computational graph.
_The below equation is the same as y = 2 * x + 3 at x = 4_ 
y = w * x + b 

### Compute gradients
_When call backward() method on y, we obtain the gradient of y according to w, x and b._  
y.backward()  

_That mean_  
VARIABLE|GRAD|SHAPE  
---|---|---  
x|tensor(2.)|tensor.Size([])  
w|tensor(4.)|tensor.Size([])
b|tensor(1.)|tensor.Size([])


