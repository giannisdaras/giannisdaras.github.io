---
permalink: /
title: ""
layout: single
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a third year Computer Science Ph.D. student at UT Austin, supervised by Prof. [Alexandros Dimakis](https://users.ece.utexas.edu/~dimakis/).

 


I am doing research on deep generative models. 
My main goal is to explore the theoretical and practical limits of solving inverse problems using deep generative priors.
I am interested in improving many aspects of deep generative models that could be useful for achieving that goal, such as fairness, high-quality sample generation, out-of-distribution generation, controllable synthesis, etc.
Application wise, I hope that my research on inverse problems with generative priors will prove useful to important real-world applications, e.g. MRI scans.

During Summer 2022, I interned at Google Research with [Peyman Milanfar](https://scholar.google.com/citations?user=iGzDl8IAAAAJ&hl=en), [Mauricio Delbracio](https://scholar.google.com/citations?user=lDDm920AAAAJ&hl=en) and [Hossein Talebi](https://scholar.google.com/citations?user=UOX9BigAAAAJ&hl=en). Prior to this internship, I worked as a Research Intern at Google with [Vincent Chu](https://scholar.google.com/citations?user=R-OrlSgAAAAJ&hl=en) and [Abhishek Kumar](https://scholar.google.com/citations?user=6vghMS0AAAAJ&hl=en).
Before joining the Ph.D., I received my undergraduate degree in ECE from the National Technical University of Athens (NTUA).
During my undergraduate studies, I worked as a Machine Learning Researcher in ExplosionAI and I successfully completed Google Summer of Code 2018.

## News
- <span style="color:blue"> [New paper]:</span> [Soft Diffusion: Score Matching for General Corruptions](https://arxiv.org/abs/2209.05442).
- <span style="color:green">[Paper acceptance]:</span> [Multitasking Models are Robust to Structural Failure: A Neural Model for Bilingual Cognitive Reserve](https://arxiv.org/abs/2210.11618), got accepted to **NeurIPS 2022**.
<!-- - <span style="color:blue">[New paper]:</span> We discovered that DALLE-2 has a secret vocabulary. We wrote a paper summarizing our findings.
Find the paper [here](https://arxiv.org/abs/2206.00169). -->
- <span style="color:green">[Paper acceptance]:</span> Our paper, [Score-Guided Intermediate Layer Optimization](https://arxiv.org/abs/2206.09104), got accepted to **ICML 2022**.





## Publications
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}
