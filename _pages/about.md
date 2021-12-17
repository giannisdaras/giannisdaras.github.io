---
permalink: /
title: ""
layout: single
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a second year Computer Science Ph.D. student at UT Austin, supervised by Prof. [Alexandros Dimakis](https://users.ece.utexas.edu/~dimakis/).

 


I am doing research on deep generative models. 
My main goal is to explore the theoretical and practical limits of solving inverse problems using deep generative priors.
I am interested in improving many aspects of deep generative models that could be useful for achieving that goal, such as fairness, high-quality sample generation, out-of-distribution generation, controllable synthesis, etc.
Application wise, I hope that my research on inverse problems with generative priors will prove useful to important real-world applications, e.g. MRI scans.

Starting from January 2022, I will be working part-time at Google Research with [Peyman Milanfar](https://scholar.google.com/citations?user=iGzDl8IAAAAJ&hl=en), [Mauricio Delbracio](https://scholar.google.com/citations?user=lDDm920AAAAJ&hl=en) and [Hossein Talebi](https://scholar.google.com/citations?user=UOX9BigAAAAJ&hl=en). Prior to this, I worked as a Research Intern at Google with [Vincent Chu](https://scholar.google.com/citations?user=R-OrlSgAAAAJ&hl=en), [Abhishek Kumar](https://scholar.google.com/citations?user=6vghMS0AAAAJ&hl=en) and [Dmitry Lagun](https://scholar.google.com/citations?user=sY8lt7AAAAAJ&hl=en). 
Before joining the Ph.D., I received my undergraduate degree in ECE from the National Technical University of Athens (NTUA).
During my undergraduate studies, I worked as a Machine Learning Researcher in ExplosionAI and I successfully completed Google Summer of Code 2018.

## News
- \[New paper\]: [Solving Inverse Problems with NerfGANs](https://arxiv.org/abs/2112.09061)
- \[Personal update\]: I joined Google as a Student Researcher working on NeRFs.
- \[Paper update\]: Our paper, Robust Compressed Sensing MRI with Deep Generative Priors, has been accepted to NeurIPS 2021.
- \[New paper\]: [Robust Compressed Sensing MRI with Deep Generative Priors](https://arxiv.org/abs/2108.01368)
- \[Paper update\]: Intermediate Layer Optimization for Inverse Problems Using Deep Generative Models, has been acceepted to ICML 2021.




## Publications
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}