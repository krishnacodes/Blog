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
Existing approaches treat depth prediction as a supervised regression problem and as a result, require vast quantities of corresponding ground truth depth data for training. This paper replaces the use of explicit depth data during training with easier-to-obtain binocular stereo footage.

## Motivation
Just recording quality depth data in a range of environments is a challenging problem. A novel training objective that enables our convolutional neural network to learn to perform single image depth estimation, despite the absence of ground truth depth data


## Detailed Summary
* Exploiting epipolar geometry constraints, disparity is generated using the image reconstruction loss.
* Training loss is a weighted sum of apperance matching loss, disparity smoothness loss, left-right disparity consistency loss.
* Exploit the ease with which binocular stereo data can be captured.
* This model can generalize to unseen datasets and still produce visually plausible depth maps


## Novelty and Contributions
* L R Consistency 

![Up conv]({{site.baseurl}}/assets/img/15adrefdsa.png)
* Training objective that allows the network to estimate single image depth in the absence of ground truth data.

## Network Details
![Network figure]({{site.baseurl}}/assets/img/4143FSD.png)
* Network uses the hour glass type architecture .
* ResNet 50 is used as the encoder part of the network .
* Decoder part appends the predictions at each resolution for making predictions at the next higher resolution.




## Results
![Results]({{site.baseurl}}/assets/img/RWGFfdsSDV43.png)


![Results]({{site.baseurl}}/assets/img/raegafd24.png)

## Authours
Clément Godard, Oisin Mac Aodha, Gabriel J. Brostow

## Sources
[Paper](https://arxiv.org/abs/1609.03677)

[Code](http://visual.cs.ucl.ac.uk/pubs/monoDepth/)