---
layout: page
title: "DiffEM: Learning from Corrupted Data with Diffusion Models via Expectation Maximization"
permalink: /publication/diffem/
nav: false
---

<p class="pub-authors">Danial Hosseintabar, Fan Chen, Giannis Daras, Antonio Torralba, Constantinos Daskalakis</p>
<p class="pub-venue">Preprint</p>
<p class="pub-links"><a href="https://arxiv.org/abs/2510.12691">Paper</a> <a href="https://github.com/danialht/DiffEM">Code</a></p>

---

> Diffusion models have emerged as powerful generative priors for high-dimensional inverse problems, yet
learning them when only corrupted or noisy observations are available remains challenging. In this work, we
propose a new method for training diffusion models with Expectation-Maximization (EM) from corrupted
data. Our proposed method, DiffEM, utilizes conditional diffusion models to reconstruct clean data from
observations in the E-step, and then uses the reconstructed data to refine the conditional diffusion model in
the M-step. Theoretically, we provide monotonic convergence guarantees for the DiffEM iteration, assuming
appropriate statistical conditions. We demonstrate the effectiveness of our approach through experiments
on various image reconstruction tasks
