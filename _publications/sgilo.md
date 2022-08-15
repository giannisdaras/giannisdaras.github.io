---
title: "Score-Guided Intermediate Layer Optimization: Fast Langevin Mixing for Inverse Problems"
collection: publications
permalink: /publication/sgilo
excerpt: ''
status: 'Published'
venue: ICML 2022
authors: '<strong> Giannis Daras (*) </strong>, Yuval Dagan (*), Alexandros G. Dimakis, Constantinos Daskalakis'
paperurl: https://arxiv.org/abs/2206.09104
date: 2022-08-04
---



> We prove fast mixing and characterize the stationary distribution of the Langevin Algorithm for inverting random weighted DNN generators. This result extends the work of Hand and Voroninski from efficient inversion to efficient posterior sampling. In practice, to allow for increased expressivity, we propose to do posterior sampling in the latent space of a pre-trained generative model. To achieve that, we train a score-based model in the latent space of a StyleGAN-2 and we use it to solve inverse problems. Our framework, Score-Guided Intermediate Layer Optimization (SGILO), extends prior work by replacing the sparsity regularization with a generative prior in the intermediate layer. Experimentally, we obtain significant improvements over the previous state-of-the-art, especially in the low measurement regime.

![](https://github.com/giannisdaras/sgilo/blob/main/paper_figs/figure1.png?raw=true)



We use diffusion models to regularize the solutions of GANs for inverse problems (e.g. inpainting, colorization, denoising, etc). 



A GAN can be decomposed into multiple intermediate generators, e.g. $G_1, G_2$ as shown below.

![](https://github.com/giannisdaras/sgilo/blob/main/paper_figs/figure2.png?raw=true)

$G_1$ typically has a low-dimensional input space which limits the expressitivity of the whole generator. 

ILO [[1]](https://arxiv.org/abs/2102.07364), [[2]](https://github.com/giannisdaras/ilo) proposes to throw away $G_1$ (after training) and optimize over the input space of $G_2$, constrained in an $l_1$ expansion of the range of $G_1$. The set of potential solutions to an inverse problem is the green shaded area shown above.

We argue that this handcrafted sparse prior can be replaced with a more powerful neural prior, coming from score-based/diffusion models. Specifically, we learn the distribution of latents in the input space of $G_2$ that correspond to natural images.     
In the figure, this is shown with the red level sets. We use the score network to regularize solutions of inverse problems in the input space of $G_2$.



Combining StyleGAN with a diffusion latent model yields a powerful image prior that can be used for many different purposes.

For example, we can use the model for image generation:


![](https://github.com/giannisdaras/sgilo/blob/main/paper_figs/generations.png?raw=true)


We can also use the prior to invert and then naturalize portraits:

![](https://github.com/giannisdaras/sgilo/blob/main/paper_figs/naturalizations.png?raw=true)



If you find this work useful, please consider citing the following papers:

```bib
@misc{daras_dagan_2022score,
    title={Score-Guided Intermediate Layer Optimization: Fast Langevin Mixing for Inverse Problems},
    author={Giannis Daras and Yuval Dagan, Alexandros G. Dimakis, Constantinos Daskalakis},
    year={2022},
    eprint={4362205},
    archivePrefix={arXiv},
    primaryClass={cs.LG}
}
```

```bib
@misc{daras2021intermediate,
    title={Intermediate Layer Optimization for Inverse Problems using Deep Generative Models},
    author={Giannis Daras and Joseph Dean and Ajil Jalal and Alexandros G. Dimakis},
    year={2021},
    eprint={2102.07364},
    archivePrefix={arXiv},
    primaryClass={cs.LG}
}
```

```bib
@inproceedings{
  song2021scorebased,
  title={Score-Based Generative Modeling through Stochastic Differential Equations},
  author={Yang Song and Jascha Sohl-Dickstein and Diederik P Kingma and Abhishek Kumar and Stefano Ermon and Ben Poole},
  booktitle={International Conference on Learning Representations},
  year={2021},
  url={https://openreview.net/forum?id=PxTIG12RRHS}
}
``` 