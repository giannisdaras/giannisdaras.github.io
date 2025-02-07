---
title: "Ambient Diffusion Posterior Sampling: Solving Inverse Problems with Diffusion Models trained on Corrupted Data"
collection: publications
permalink: /publication/ambient_dps
excerpt: ''
status: 'Published'
venue: 'ICLR 2025'
authors: Asad Aali, <strong> Giannis Daras</strong>, Brett Levac, Sidharth Kumar, Alexandros G. Dimakis, Jonathan I. Tamir'
paperurl: https://arxiv.org/abs/2403.08728
code: https://github.com/utcsilab/ambient-diffusion-mri
date: 2024-11-01
---

![](https://github.com/asad-aali/ambient-diffusion-mri/raw/main/docs/all_priors.png)

> We provide a framework for solving inverse problems with diffusion models learned from linearly corrupted data. Our method, Ambient Diffusion Posterior Sampling (A-DPS), leverages a generative model pre-trained on one type of corruption (e.g. image inpainting) to perform posterior sampling conditioned on measurements from a potentially different forward process (e.g. image blurring). We test the efficacy of our approach on standard natural image datasets (CelebA, FFHQ, and AFHQ) and we show that A-DPS can sometimes outperform models trained on clean data for several image restoration tasks in both speed and performance. We further extend the Ambient Diffusion framework to train MRI models with access only to Fourier subsampled multi-coil MRI measurements at various acceleration factors (R = 2, 4, 6, 8). We again observe that models trained on highly subsampled data are better priors for solving inverse problems in the high acceleration regime than models trained on fully sampled data.



Please read the [paper](https://arxiv.org/abs/2403.08728) for more details.