---
layout: post-wo-sidebar
title: Deep CORAL :Correlation Alignment for Deep Domain Adaptation [ECCV-W 16]
date: 2017-12-11 15:47:20 +0300
description: 
img: dffdsafsadfas.png
content_type: domain_adaptation
tags: [Domain Adaptation]
---


## One Line Summary
* Deep neural networks don't generalize well when the source and target data distributions are different, this work performs the domain adaptation by aligning the second order statistics.

## Motivation
* Many machine learning algorithms assume that training and test data are independent and identically distributed, However, this assumption rarely holds in practice as the data is likely to change over time and space. 


## Detailed Summary
* The Network has the classification loss on the source domain for good classification accuracy
* There is a CORAL loss for making the network extract the domain independent features and generalize well across domains.

## Novelty and Contributions
* Address the unsupervised domain adaptation where there are no labelled training data in the target domain.
* Minimize the difference in second-order statistics between the source and target feature activations.


## Network Details
![Network]({{site.baseurl}}/assets/img/dffdsafsadfas.png)

* The Network the shared weights across the two domains, as we are trying to capture the domain independent representation. 

## Results
![Results]({{site.baseurl}}/assets/img/fdsafsfsfdsa.png)


![Results]({{site.baseurl}}/assets/img/fdsdfsafasdfdsa.png)

## Authors
Baochen Sun, Kate Saenko

## Sources
[Paper](https://arxiv.org/abs/1607.01719)
