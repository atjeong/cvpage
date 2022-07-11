---
title: "BiasEnsemble: Revisiting the Importance of
Amplifying Bias for Debiasing"
date: 2022-07-11T16:43:25+09:00
draft: true
---

### <center>Jungsoo Lee\*, <span style="color: #6693F5">Jeonghoon Park\*</span>, Daeyoung Kim\*, Junyoung Lee, Edward Choi, Jaegul Choo</center>

---

## Abstract

In image classification, "debiasing" aims to train a classifier to be less susceptible to dataset bias, the strong correlation between peripheral attributes of data samples and a target class. For example, even if the frog class in the dataset mainly consists of frog images with a swamp background (i.e., bias-aligned samples), a debiased classifier should be able to correctly classify a frog at a beach (i.e., bias-conflicting samples). Recent debiasing approaches commonly use two components for debiasing, a biased model fB and a debiased model fD. fB is trained to focus on bias-aligned samples while fD is mainly trained with bias-conflicting samples by concentrating on samples which fB fails to learn, leading fD to be less susceptible to the dataset bias. While the state-of-the-art debiasing techniques have aimed to better train fD, we focus on training fB, an overlooked component until now. Our empirical analysis reveals that removing the bias-conflicting samples from the training set for fB is important for improving the debiasing performance of fD. This is due to the fact that the bias-conflicting samples work as noisy samples for amplifying the bias for fB. To this end, we propose a novel biased sample selection method BiasEnsemble which removes the bias-conflicting samples via leveraging additional biased models to construct a bias-amplified dataset for training fB. Our simple yet effective approach can be directly applied to existing reweighting-based debiasing approaches, obtaining consistent performance boost and achieving the state-of-the-art performance on both synthetic and real-world datasets.

---

## Method Overview

![image-20220711170219161](/images/BE_overview.pdf)

---

## Quantitative Results

---

## Links

📍 [ArXiv](https://arxiv.org/abs/2205.14594)

