---
permalink: /
title: ""
layout: single
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a fourth year Computer Science Ph.D. student at UT Austin, supervised by Prof. [Alexandros Dimakis](https://users.ece.utexas.edu/~dimakis/).

 


I am doing research on deep generative models. 
My main goal is to explore the theoretical and practical limits of solving inverse problems using deep generative priors.
I am interested in improving many aspects of deep generative models that could be useful for achieving that goal, such as fairness, high-quality sample generation, out-of-distribution generation, controllable synthesis, etc.
Application wise, I hope that my research on inverse problems with generative priors will prove useful to important real-world applications, e.g. accelerating MRI.

During Summer 2022, I interned at Google Research with [Peyman Milanfar](https://scholar.google.com/citations?user=iGzDl8IAAAAJ&hl=en), [Mauricio Delbracio](https://scholar.google.com/citations?user=lDDm920AAAAJ&hl=en) and [Hossein Talebi](https://scholar.google.com/citations?user=UOX9BigAAAAJ&hl=en). Prior to this internship, I worked as a Research Intern at Google with [Vincent Chu](https://scholar.google.com/citations?user=R-OrlSgAAAAJ&hl=en) and [Abhishek Kumar](https://scholar.google.com/citations?user=6vghMS0AAAAJ&hl=en).
Before joining the Ph.D., I received my undergraduate degree in ECE from the National Technical University of Athens (NTUA).
During my undergraduate studies, I worked as a Machine Learning Researcher in ExplosionAI and I successfully completed Google Summer of Code 2018.

## News
- <span style="color:blue"> [Personal News]: </span> I am joining NVIDIA as Research Scientist Intern.
- <span style="color:green"> [Paper Acceptance]: </span> [Ambient Diffusion: Learning Clean Distributions from Corrupted Data](https://arxiv.org/abs/2305.19256) got accepted to **NeurIPS 2023**.
- <span style="color:green"> [Paper Acceptance]: </span> [Consistent Diffusion Models: Mitigating Sampling Drift by Learning to be Consistent](https://arxiv.org/abs/2302.09057) got accepted to **NeurIPS 2023**.
- <span style="color:green"> [Paper Acceptance]: </span> [Solving Linear Inverse Problems Provably via Posterior Sampling with Latent Diffusion Models
](https://arxiv.org/abs/2307.00619) got accepted to **NeurIPS 2023**.
- <span style="color:green"> [Paper Acceptance]: </span> [DataComp: In search of the next generation of multimodal datasets](https://arxiv.org/abs/2304.14108) got accepted to **NeurIPS 2023 (Oral)**.
- <span style="color:green"> [Paper acceptance]: </span> [Restoration-degradation beyond linear diffusions: A non-asymptotic analysis for DDIM-type samplers](https://arxiv.org/abs/2303.03384) got accepted to **ICML 2023**.
- <span style="color:green"> [Paper acceptance]: </span> [Soft Diffusion: Score Matching for General Corruptions](https://arxiv.org/abs/2209.05442) got accepted to **TMLR**.
- <span style="color:green"> [Paper acceptance]: </span> [Discovering the Hidden Vocabulary of DALLE-2](https://arxiv.org/abs/2206.00169) got accepted to the **NeurIPS 2022 Workshop on Score-Based Methods**.
- <span style="color:green">[Paper acceptance]:</span> [Multitasking Models are Robust to Structural Failure: A Neural Model for Bilingual Cognitive Reserve](https://arxiv.org/abs/2210.11618) got accepted to **NeurIPS 2022**.
- <span style="color:green">[Paper acceptance]:</span> Our paper, [Score-Guided Intermediate Layer Optimization](https://arxiv.org/abs/2206.09104), got accepted to **ICML 2022**.





## Publications
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}
