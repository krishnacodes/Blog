---
layout: post-wo-sidebar
title: Fast Feature Fool [BMVC 17]
date: 2017-12-07 15:47:20 +0300
description: 
img: dfdsdsadfd.png
content_type: adversarial_training
tags: [Adversarial Perturbations, VAL]
---


## One Line Summary
* A data independent approach to universal adversarial perturbations

## Motivation
* For an attacker to have access to the training data is not practical making the attacks unsuitable for real world scenarios.

## Detailed Summary
* State-of-the-art object recognition Convolutional Neural Networks (CNNs) are shown to be fooled by image agnostic perturbations, called universal adversarial perturbations.
* It is also observed that these perturbations generalize across multiple networks trained on the same target data. However, these algorithms require training data on which the CNNs
were trained and compute adversarial perturbations via complex optimization. 
* The fooling performance of these approaches is directly proportional to the amount of available training data.
* Novel data independent image agnostic approach is proposed to alleviate this limitation

## Novelty and Contributions
* Fooling the target classifier without using the data.
* Excellent cross model generalizability and first model to use data independent approach for adversarial perturbation generation.


## Network Details

* multiple CNN architectures trained on ILSVRC dataset.
* CaffeNet (similar to Alexnet), VGG-F, VGG-16, VGG-19 and GoogLeNet architectures.
![Results]({{site.baseurl}}/assets/img/dfddd4425q24.png)

## Results
![Results]({{site.baseurl}}/assets/img/dfdsdsadfd.png)


![Results]({{site.baseurl}}/assets/img/dsfaddafddf.png)

## Authors
Konda Reddy Mopuri, Utsav Garg, R. Venkatesh Babu

## Sources
[Paper](https://arxiv.org/abs/1707.05572)

[Code](https://github.com/utsavgarg/fast-feature-fool)
