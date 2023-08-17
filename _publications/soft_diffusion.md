---
title: "Soft Diffusion: Score Matching for General Corruptions"
collection: publications
permalink: /publication/soft_diffusion
excerpt: ''
status: 'Published'
venue: 'TMLR 2023'
authors: '<strong> Giannis Daras</strong>, Mauricio Delbracio, Hossein Talebi, Alexandros G. Dimakis, Peyman Milanfar'
paperurl: https://arxiv.org/abs/2209.05442
date: 2022-10-21
---

![](../images/soft_diffusion.png)


> We define a broader family of corruption processes that generalizes previously known diffusion models. To reverse these general diffusions, we propose a new objective called Soft Score Matching that provably learns the score function for any linear corruption process and yields state of the art results for CelebA. Soft Score Matching incorporates the degradation process in the network. Our new loss trains the model to predict a clean image, *that after corruption*, matches the diffused observation. We show that our objective learns the gradient of the likelihood under suitable regularity conditions for a family of corruption processes. We further develop a principled way to select the corruption levels for general diffusion processes and a novel sampling method that we call Momentum Sampler. We show experimentally that our framework works for general linear corruption processes, such as Gaussian blur and masking. We achieve state-of-the-art FID score 1.85 on CelebA-64, outperforming all previous linear diffusion models. We also show significant computational benefits compared to vanilla denoising diffusion.



Please read the [paper](https://arxiv.org/abs/2209.05442) for more details.

