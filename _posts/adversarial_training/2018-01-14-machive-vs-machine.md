---
layout: post-wo-sidebar
title: Machine vs Machine :Minimax-Optimal Defense Against Adversarial Examples [NIPS-W 17]
date: 2018-01-10 15:47:20 +0300
description: 
img: fdsafdsafads.png
content_type: adversarial_training
tags: [Adversarial Perturbations]
---


## One Line Summary
* Adversarial training of the classifier with the perturbations generated using the attack network

## Motivation
* Since recent works have shown that adversarial perturbations can be generated using the neural networks, the target classifiers can be made robust to these attacks by GAN training for target classifier with these perturbations

## Detailed Summary
* Propose a sensitivity-penalized optimization method to numerically find continuous minimax solutions, which is better than alternating descent/ascent. The proposed optimization method can also be used for other minimax problems beyond the adversarial example problem.

## Novelty and Contributions
* A continuous game model to analyze adversarial example attacks and defenses, using the neural network-based attack class as a feasible approximation to a larger but intractable class of optimization-based attacks.

* Demonstrate the difficulty of defending against multiple attack types and present the
minimax defense as the best worst-case defense methods.


## Network Details

* The attack network (AttNet), can be of any class of appropriate neural networks. Here a three-layer fully-connected network with 300 hiddens units per layer

## Results
![Results]({{site.baseurl}}/assets/img/dfadafadd.png)


![Results]({{site.baseurl}}/assets/img/fsafsdafsafads.png)

## Authors
Jihun Hamm

## Sources
[Paper](https://arxiv.org/abs/1711.04368)
