---
title: "Ambient Dataloops: Generative Models for Dataset Refinement"
collection: publications
permalink: /publication/ambient_dataloops
excerpt: ''
status: 'Published'
venue: 'ICML 2026'
authors: 'Adrián Rodríguez-Muñoz, William Daspit, Adam Klivans, Antonio Torralba, Constantinos Daskalakis, <strong>Giannis Daras</strong>'
paperurl: https://arxiv.org/abs/2601.15417
date: 2026-01-21
---

> We propose Ambient Dataloops, an iterative framework for refining datasets that makes it easier for diffusion models to learn the underlying data distribution. Modern datasets contain samples of highly varying quality, and training directly on such heterogeneous data often yields suboptimal models. We propose a dataset-model co-evolution process; at each iteration of our method, the dataset becomes progressively higher quality, and the model improves accordingly. To avoid destructive self-consuming loops, at each generation, we treat the synthetically improved samples as noisy, but at a slightly lower noisy level than the previous iteration, and we use Ambient Diffusion techniques for learning under corruption. Empirically, Ambient Dataloops achieve state-of-the-art performance in unconditional and text-conditional image generation and de novo protein design. We further provide a theoretical justification for the proposed framework that captures the benefits of the data looping procedure.

Please read the [paper](https://arxiv.org/abs/2601.15417) for more details.
