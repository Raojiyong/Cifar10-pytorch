## Cifar10 with pytorch

This is the Pytorch implementation of LeNet and ResNet18 network trained on CIFAR10 dataset

## Introduction

dataset :[download](http://www.cs.toronto.edu/~kriz/cifar.html)

The CIFAR-10 dataset consists of 60000 32x32 colour images in 10 classes, with 6000 images per class. There are 50000 training images and 10000 test images.

The dataset is divided into five training batches and one test batch, each with 10000 images. The test batch contains exactly 1000 randomly-selected images from each class. The training batches contain the remaining images in random order, but some training batches may contain more images from one class than another. Between them, the training batches contain exactly 5000 images from each class.

## Requirement

- python3.6+
- numpy
- pytorch1.8.1+cu111
- torchvision0.9.0

## Usage

`run Lenet.ipynb`

`run resnet18.ipynb`

## Results

|          | epochs | optimizer | lr   | train_acc | valid_acc | test_acc |
| -------- | ------ | --------- | ---- | --------- | --------- | -------- |
| LeNet    | 50     | Adam      | 0.01 | 85.43%    | 61.50%    | 61.39%   |
|          | 50     | SGD       | 0.01 | 68.01%    | 62.97%    | 62.97%   |
| ResNet18 | 30     | Adam      | 0.01 | 98.39%    | 80.50%    | 80.50%   |
|          | 30     | SGD       | 0.01 | 98.13%    | 82.00%    | 81.54%   |





