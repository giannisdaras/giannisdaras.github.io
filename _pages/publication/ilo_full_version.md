---
layout: page
title: "Intermediate Layer Optimization for Inverse Problems using Deep Generative Models"
permalink: /publication/ilo/
nav: false
---

<p class="pub-authors">Giannis Daras, Joseph Dean, Ajil Jalal, Alexandros G. Dimakis</p>
<p class="pub-venue">ICML 2021</p>
<p class="pub-links"><a href="https://arxiv.org/abs/2102.07364">Paper</a> <a href="https://github.com/giannisdaras/ilo">Code</a></p>

---

We propose Intermediate Layer Optimization (ILO), a novel optimization algorithm for solving inverse problems with deep generative models. Instead of optimizing only over the initial latent code, we progressively change the input layer obtaining successively more expressive generators. To explore the higher dimensional spaces, our method searches for latent codes that lie within a small l1 ball around the manifold induced by the previous layer. Our theoretical analysis shows that by keeping the radius of the ball relatively small, we can improve the established error bound for compressed sensing with deep generative models. We empirically show that our approach outperforms state-of-the-art methods introduced in StyleGAN-2 and PULSE for a wide range of inverse problems including inpainting, denoising, super-resolution and compressed sensing.


### Inpainting
![](/assets/img/ilo_inpainting.png)


### Super-resolution
![](/assets/img/ilo_super_res.png)

### Denoising
![](/assets/img/ilo_denoising.png)

### Morphing using a robust classifier
![](/assets/img/ilo_morphing.png)
