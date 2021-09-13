---
permalink: /
title: ""
layout: single
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

## About me

I am a second year Computer Science Ph.D. student at UT Austin.
I am honored to be supervised by Prof. [Alexandros Dimakis](https://users.ece.utexas.edu/~dimakis/).


Currently, I am working as a Student Researcher at Google Research with [Vincent Chu](https://scholar.google.com/citations?user=R-OrlSgAAAAJ&hl=en), [Abhishek Kumar](https://scholar.google.com/citations?user=6vghMS0AAAAJ&hl=en) and [Dmitry Lagun](https://scholar.google.com/citations?user=sY8lt7AAAAAJ&hl=en).


I am doing research on deep generative models. 
My main goal is to explore the theoretical and practical limits of solving inverse problems using deep generative priors.
I am interested in improving many aspects of deep generative models that could be useful for achieving that goal, such as fairness, high-quality sample generation, out-of-distribution generation, controllable synthesis, etc.
Application wise, I hope that my research on inverse problems with generative priors will prove useful to important real-world applications, e.g. MRI scans.

Before joining the Ph.D., I received my undergraduate degree in ECE from National Technical University of Athens (NTUA).
During my undergraduate studies, I worked as a Machine Learning Researcher in ExplosionAI.
and I successfully completed Google Summer of Code 2018.

## News
- I joined Google as a Student Researcher working on NeRFs.
- New paper alert: [Robust Compressed Sensing MRI with Deep Generative Priors](https://arxiv.org/abs/2108.01368)
- Our paper, Intermediate Layer Optimization for Inverse Problems Using Deep Generative Models, has been acceepted to ICML 2021.
- I am serving as a reviewer for NeurIPS 2021.
- This summer, I will join Google Research for an internship on generative models!
- I am serving as a reviewer for ICML 2021.


## Publications
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}