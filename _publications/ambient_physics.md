---
title: "Ambient Physics: Training Neural PDE Solvers with Partial Observations"
collection: publications
permalink: /publication/ambient_physics
excerpt: ''
status: 'Preprint'
authors: 'Harris Abdul Majid, <strong>Giannis Daras</strong>, Francesco Tudisco, Steven McDonagh'
paperurl: https://arxiv.org/abs/2602.13873
date: 2026-02-14
---

> In many scientific settings, acquiring complete observations of PDE coefficients and solutions can be expensive, hazardous, or impossible. Recent diffusion-based methods can reconstruct fields given partial observations, but require complete observations for training. We introduce Ambient Physics, a framework for learning the joint distribution of coefficient-solution pairs directly from partial observations, without requiring a single complete observation. The key idea is to randomly mask a subset of already-observed measurements and supervise on them, so the model cannot distinguish "truly unobserved" from "artificially unobserved", and must produce plausible predictions everywhere. Ambient Physics achieves state-of-the-art reconstruction performance. Compared with prior diffusion-based methods, it achieves a 62.51% reduction in average overall error while using 125× fewer function evaluations. We also identify a "one-point transition": masking a single already-observed point enables learning from partial observations across architectures and measurement patterns. Ambient Physics thus enables scientific progress in settings where complete observations are unavailable.

Please read the [paper](https://arxiv.org/abs/2602.13873) for more details.
