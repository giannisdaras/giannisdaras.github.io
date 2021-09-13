---
title: "Robust Compressed Sensing MRI with Deep Generative Priors"
collection: publications
permalink: /publication/mri
excerpt: ''
status: 'Preprint'
venue: arXiv
authors: 'Ajil Jalal, Marius Arvinte, <strong> Giannis Daras </strong>, Eric Price, Alexandros G. Dimakis, Jonathan I. Tamir'
code: 'https://github.com/utcsilab/csgm-mri-langevin'
paperurl: https://arxiv.org/abs/2108.01368
date: 2021-02-15
---
The CSGM framework (Bora-Jalal-Price-Dimakis'17) has shown that deep generative priors can be powerful tools for solving inverse problems. However, to date this framework has been empirically successful only on certain datasets (for example, human faces and MNIST digits), and it is known to perform poorly on out-of-distribution samples. In this paper, we present the first successful application of the CSGM framework on clinical MRI data. We train a generative prior on brain scans from the fastMRI dataset, and show that posterior sampling via Langevin dynamics achieves high quality reconstructions. Furthermore, our experiments and theory show that posterior sampling is robust to changes in the ground-truth distribution and measurement process.


![](../images/mri_main.jpg)