---
permalink: /
title: ""
layout: single
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a post-doc at MIT CSAIL, working closely with [Prof. Costantinos Daskalakis](https://people.csail.mit.edu/costis/) and [Prof. Antonio Torralba](https://groups.csail.mit.edu/vision/torralbalab/).

Prior to that, I spent 4 wonderful years at UT Austin, working with [Prof. Alexandros Dimakis](https://users.ece.utexas.edu/~dimakis/). 

Before starting my Ph.D., I received my undergraduate degree in ECE from the National Technical University of Athens (NTUA).

 

My research is on generative modeling. I am particularly interested in the problem of learning generative models from corrupted data.



## News
- <span style="color:green"> [Best Contribution Award]: </span> [Best Contribution Award](https://baspfrontiers.org/best-contribution-awards/) at the International Biomedical and Astronomical Signal Processing ([BASP](https://baspfrontiers.org/)) Frontiers Conference 2025.
![](images/basp2025.jpg)
- <span style="color:green"> [Paper Acceptance]: </span> [How Much is a Noisy Image Worth?](https://arxiv.org/abs/2411.02780) got accepted to **ICLR 2025**.
- <span style="color:green"> [Paper Acceptance]: </span> [Ambient Diffusion Posterior Sampling](https://arxiv.org/abs/2403.08728) got accepted to **ICLR 2025**.
- <span style="color:green"> [Paper Acceptance]: </span> [Infilling Score](https://openreview.net/forum?id=9QPH1YQCMn) got accepted to **ICLR 2025**.



**Internships**:
* NVIDIA Research (2023) with [Arash Vahdat](https://scholar.google.com/citations?user=p9-nlRIAAAAJ&hl=en).
* Google Research (2022) with [Peyman Milanfar](https://scholar.google.com/citations?user=iGzDl8IAAAAJ&hl=en), [Mauricio Delbracio](https://scholar.google.com/citations?user=lDDm920AAAAJ&hl=en) and [Hossein Talebi](https://scholar.google.com/citations?user=UOX9BigAAAAJ&hl=en). 
* Google Research (2022) with [Vincent Chu](https://scholar.google.com/citations?user=R-OrlSgAAAAJ&hl=en) and [Abhishek Kumar](https://scholar.google.com/citations?user=6vghMS0AAAAJ&hl=en).






## Publications
For a more comprehensive list of publications, please visit my [Google Scholar](https://scholar.google.com/citations?user=LaScvbQAAAAJ&hl=en) page.
{% include base_path %}

{% assign sorted = site.publications | reverse %}
{% for post in sorted %}
  {% include archive-single.html %}
{% endfor %}
