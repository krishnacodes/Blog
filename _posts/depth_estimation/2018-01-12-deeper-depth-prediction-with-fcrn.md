---
layout: post-wo-sidebar
title: Deeper Depth Prediction with Fully Convolutional Residual Networks[3DV 16]
date: 2017-12-03 15:47:20 +0300
description: 
img: 2345.png
tags: [3DV, 3DV16, Depth Estimation]
content_type: depth_estimaiton
---



## One Line Summary
Depth estimation using a fully convolutional architecture optimized using a reverse Huber loss without any post processing steps, showing the state of the art result on benchmark datasets.

## Motivation
Encoder-decoder architectures uses the high level and low level features for optimal predictions, since depth estimation requires global and local uses, this architecture is well for suited depth estimation task.


## Detailed Summary
* A novel approach to the problem of depth estimation from a single image, single-scale CNN architecture that follows residual learning. The proposed network is fully convolutional, comprising up-projection layers that allow for training much deeper configurations, illustrates a faster and
more efficient approach to up-convolutional layers, berHu loss is used for the better convergence.


## Novelty and Contributions
* Reverse Huber loss is introduced(berHu loss)
* Faster up convolutions, up projections are  a faster implementaiton of up convolutions 
![Up conv]({{site.baseurl}}/assets/img/2345.png)



## Network Details
![Network figure]({{site.baseurl}}/assets/img/564323.png)
* Network uses the encoder-decoder architecture to capture both high level features and the low level features.
* ResNet 50 is used as the encoder part of the network .
* Decoder part contains the up projections.




## Results
![Results]({{site.baseurl}}/assets/img/4t3eafdfga.png)


![Results]({{site.baseurl}}/assets/img/43q543.png)

## Authours
Iro Laina, Christian Rupprecht, Vasileios Belagiannis, Federico Tombari, Nassir Navab

## Sources
[Paper](https://arxiv.org/abs/1606.00373)

[Code](https://github.com/iro-cp/FCRN-DepthPrediction)


