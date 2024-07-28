---
permalink: /
title: ""
layout: single
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a fourth year Computer Science Ph.D. student at UT Austin, supervised by Prof. [Alexandros Dimakis](https://users.ece.utexas.edu/~dimakis/). Before starting my Ph.D., I received my undergraduate degree in ECE from the National Technical University of Athens (NTUA).

 


My research is on generative modeling. I am particularly interested in the problem of learning generative models from corrupted data.


**Internships**:
* NVIDIA Research (2023) with [Arash Vahdat](https://scholar.google.com/citations?user=p9-nlRIAAAAJ&hl=en).
* Google Research (2022) with [Peyman Milanfar](https://scholar.google.com/citations?user=iGzDl8IAAAAJ&hl=en), [Mauricio Delbracio](https://scholar.google.com/citations?user=lDDm920AAAAJ&hl=en) and [Hossein Talebi](https://scholar.google.com/citations?user=UOX9BigAAAAJ&hl=en). 
* Google Research (2022) with [Vincent Chu](https://scholar.google.com/citations?user=R-OrlSgAAAAJ&hl=en) and [Abhishek Kumar](https://scholar.google.com/citations?user=6vghMS0AAAAJ&hl=en).



## News
- <span style="color:green"> [Paper Acceptance]: </span> [Consistent Diffusion Meets Tweedie](https://arxiv.org/abs/2404.10177) got accepted to **ICML 2024**.
- <span style="color:green"> [Paper Acceptance]: </span> [Ambient Diffusion: Learning Clean Distributions from Corrupted Data](https://arxiv.org/abs/2305.19256) got accepted to **NeurIPS 2023**.
- <span style="color:green"> [Paper Acceptance]: </span> [Consistent Diffusion Models: Mitigating Sampling Drift by Learning to be Consistent](https://arxiv.org/abs/2302.09057) got accepted to **NeurIPS 2023**.
- <span style="color:green"> [Paper Acceptance]: </span> [Solving Linear Inverse Problems Provably via Posterior Sampling with Latent Diffusion Models
](https://arxiv.org/abs/2307.00619) got accepted to **NeurIPS 2023**.
- <span style="color:green"> [Paper Acceptance]: </span> [DataComp: In search of the next generation of multimodal datasets](https://arxiv.org/abs/2304.14108) got accepted to **NeurIPS 2023 (Oral)**.
- <span style="color:green"> [Paper acceptance]: </span> [Restoration-degradation beyond linear diffusions: A non-asymptotic analysis for DDIM-type samplers](https://arxiv.org/abs/2303.03384) got accepted to **ICML 2023**.





## Publications
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}
