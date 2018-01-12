---
layout: post-wo-sidebar
title: Unsupervised Monocular Depth Estimation with Left-Right Consistency[CVPR 17]
date: 2017-12-04 15:47:20 +0300
description: 
img: 4143FSD.png
tags: [CVPR, CVPR17, Depth Estimation]
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
Clément Godard, Oisin Mac Aodha, Gabriel J. Brostow

## Sources
[Paper](https://arxiv.org/abs/1609.03677)

[Code](http://visual.cs.ucl.ac.uk/pubs/monoDepth/)