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

I am a first year Computer Science Ph.D. student at UT Austin.
I am honored to be supervised by Prof. [Alexandros Dimakis](https://users.ece.utexas.edu/~dimakis/).
I received my undergraduate degree in ECE from National Technical University of Athens (NTUA).
During my undergraduate studies, I worked as a Machine Learning Researcher in ExplosionAI
and I successfully completed Google Summer of Code 2018.


I am doing research on deep generative models. 
My main goal is to explore the theoretical and practical limits of solving inverse problems using deep generative priors.
I am interested in improving many aspects of deep generative models that could be useful for achieving that goal, such as fairness, high-quality sample generation, out-of-distribution generation, controllable synthesis, etc.
Application wise, I hope that my research on inverse problems with generative priors will prove useful to important real-world applications, e.g. MRI scans.

## News
- This summer, I will join Google Research for an internship on generative models!
- I am reviewing 7 papers for ICML 2021.


## Publications
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}