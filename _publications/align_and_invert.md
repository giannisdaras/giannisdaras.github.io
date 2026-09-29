---
title: "Align & Invert: Solving Inverse Problems with Diffusion and Flow-based Models via Representation Alignment"
collection: publications
permalink: /publication/align_and_invert
excerpt: ''
status: 'Published'
venue: 'NeurIPS 2026'
authors: 'Loukas Sfountouris, <strong>Giannis Daras</strong>, Paris Giampouras'
paperurl: https://arxiv.org/abs/2511.16870
code: https://github.com/Sfountouris/Align_And_Invert
date: 2025-11-21
---

> Enforcing alignment between the internal representations of diffusion or flow-based generative models and those of pretrained self-supervised encoders has recently been shown to provide a powerful inductive bias, improving both convergence and sample quality. In this work, we extend this idea to inverse problems, where pretrained generative models are employed as priors. We propose applying representation alignment (REPA) between diffusion or flow-based models and a DINOv2 visual encoder, to guide the reconstruction process at inference time. Although ground-truth signals are unavailable in inverse problems, we empirically show that aligning model representations of approximate target features can substantially enhance reconstruction quality and perceptual realism. We provide theoretical results showing (a) that REPA regularization can be viewed as a variational approach for minimizing a divergence measure in the DINOv2 embedding space, and (b) how under certain regularity assumptions REPA updates steer the latent diffusion states toward those of the clean image. These results offer insights into the role of REPA in improving perceptual fidelity. We integrate REPA into multiple state-of-the-art inverse problem solvers, and provide extensive experiments on super-resolution, box inpainting, Gaussian deblurring, and motion deblurring confirming that our method consistently improves reconstruction quality, while also providing efficiency gains reducing the number of required discretization steps.

Please read the [paper](https://arxiv.org/abs/2511.16870) for more details.
