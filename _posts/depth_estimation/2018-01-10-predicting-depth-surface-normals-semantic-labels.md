---
layout: post-wo-sidebar
title: Predicting Depth, Surface Normals and Semantic Labels with a Common Multi-Scale Convolutional Architecture [ICCV 15]
date: 2017-12-01 15:47:20 +0300
description: Depth estimation, surface normal estimaiton and semantic labeling are done using a single basic architecture without any super pixels or low level segmentation, state-of-the-art results on all three tasks are shown.
img: multi_scale_depth_eigen_iccv15.png # Add image post (optional)
tags: [ICCV15, Depth Estimation]
content_type: depth_estimaiton
---


## One Line Summary
Depth estimation, surface normal estimaiton and semantic labeling are done using a single basic architecture without any super pixels or low level segmentation, state-of-the-art results on all three tasks are shown.

## Motivation
Use of a single architecture helps simplify the implementation of systems that require multiple modalities, e.g. robotics or augmented reality, which in
turn can help enable research progress in these areas. Especially, in the case of depth and normals, much of the computation can be shared between modalities, making the system more efficient.

## Detailed Summary
Starting with coarse level predictions in first scale and then doing finer level predictions in the next scales, effectively exploting the correaltion among the tasks of depth prediction, surface normal estimaiton and semantic segmentation by sharing the first two scales for all three tasks and only third scale network being individual to each task. 


## Novelty and Contributions
* Use of the Multi-scale architecture where first and second scale are shared among different tasks
* Showing the state-of-the-art results on all three tasks hence emprically proving the correlation between the three scene understanding tasks.



## Network Details
![Network figure]({{site.baseurl}}/assets/img/multi_scale_depth_eigen_iccv15.png)
* First two scales of the network are trained jointly from the start, somewhat simplifying the training procedure and yielding performance gains.
* Predictions from each scale are fed into the next scale.



## Results

### Depth Estimation
![Results]({{site.baseurl}}/assets/img/Screenshot from 2018-01-12 12-38-19.png)
![Results]({{site.baseurl}}/assets/img/Screenshot from 2018-01-12 12-43-41.png)


### Surface Normal Estimation

![Results]({{site.baseurl}}/assets/img/Screenshot from 2018-01-12 13-50-57.png)
![Results]({{site.baseurl}}/assets/img/Screenshot from 2018-01-12 13-57-07.png)


### Semantic Segmentation


![Results]({{site.baseurl}}/assets/img/Screenshot from 2018-01-12 13-54-29.png)
![Results]({{site.baseurl}}/assets/img/Screenshot from 2018-01-12 12-41-53.png)



## Similar Works
* [Depth Map Prediction from a Single Image using a Multi-Scale Deep Network]({{site.baseurl}}/depthmap-prediction-from-a-single/)




## Authours
David Eigen, Rob Fergus

## Sources
[Paper](https://arxiv.org/abs/1411.4734)

[Code](http://cs.nyu.edu/˜deigen/dnl/)


