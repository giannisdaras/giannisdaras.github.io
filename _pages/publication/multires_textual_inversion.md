---
layout: page
title: "Multiresolution Textual Inversion"
permalink: /publication/multires_textual_inversion/
nav: false
---

<p class="pub-authors">Giannis Daras, Alexandros G. Dimakis</p>
<p class="pub-venue">NeurIPS 2022, SBM Workshop &middot; Oral</p>
<p class="pub-links"><a href="https://arxiv.org/abs/2211.17115">Paper</a> <a href="https://github.com/giannisdaras/multires_textual_inversion">Code</a></p>

---

![](/assets/img/example_dog.png)


We extend Textual Inversion to learn pseudo-words that represent a concept at different resolutions. This allows us to generate images that use the concept with different levels of detail and also to manipulate different resolutions using language.
Once learned, the user can generate images at different levels of agreement to the original concept: "*A photo of <S(0)>*" produces the exact object while the prompt: "*A photo of <S(0.8)>*" only matches the rough outlines and colors. 
Our framework allows us to generate images that use different resolutions of an image (e.g. details, textures, styles)  as separate pseudo-words that can be composed in various  ways. 



#### Fully Resolution-Dependent Sampling
![](/assets/img/fully.png)


#### Semi Resolution-Dependent Sampling
![](/assets/img/semi.png)


#### Fixed Resolution Sampling
![](/assets/img/fixed.png)



If you find this work useful, please consider citing the following papers:

```
@misc{daras2022multires,
      url = {https://arxiv.org/abs/2211.17115},
      author = {Giannis Daras and Alexandros G. Dimakis},
      title = {Multiresolution Textual Inversion},
      publisher = {arXiv},
      year = {2022},
      primaryClass={cs.CV}
}
```

```
@misc{gal2022textual,
      doi = {10.48550/ARXIV.2208.01618},
      url = {https://arxiv.org/abs/2208.01618},
      author = {Gal, Rinon and Alaluf, Yuval and Atzmon, Yuval and Patashnik, Or and Bermano, Amit H. and Chechik, Gal and Cohen-Or, Daniel},
      title = {An Image is Worth One Word: Personalizing Text-to-Image Generation using Textual Inversion},
      publisher = {arXiv},
      year = {2022},
      primaryClass={cs.CV}
}
```
