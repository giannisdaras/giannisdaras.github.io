---
title: "Ambient Diffusion Policy: Imitation Learning from Suboptimal Data in Robotics"
collection: publications
permalink: /publication/ambient_diffusion_policy
excerpt: ''
status: 'Published'
venue: 'RSS 2026 Workshops on Data-Centric Robotics and "It''s the Demos"'
authors: 'Adam Wei, Nicholas Pfaff, Thomas Cohn, Arif Kerem Dayı, Constantinos Daskalakis, <strong>Giannis Daras</strong>, Russ Tedrake'
paperurl: https://arxiv.org/abs/2606.12365
website: https://ambient-diffusion-policy.github.io/
date: 2026-06-10
awards:
  - text: 'Best Paper Award'
    venue: 'Data-Centric Robotics Workshop, RSS 2026'
    url: https://rss-workshop-2026.github.io/
  - text: 'Most Useful Practical Information Award'
    venue: '"It''s the Demos" Workshop, RSS 2026'
    url: https://its-the-demos.github.io/
---

{% include award-badges.html awards=page.awards %}

> We propose Ambient Diffusion Policy, a simple and principled method for imitation learning from suboptimal data in robotics. High-quality, task-specific robot data is expensive and time-consuming to collect, while suboptimal datasets with lower-quality or out-of-distribution demonstrations are abundant. Existing methods that co-train on both data sources in robotics often fail to separate the meaningful and the harmful features in the suboptimal samples. In contrast, our method extracts only the useful features by introducing a new axis to co-training in robotics: noise-dependent data usage. Ambient Diffusion Policy restricts the contribution of suboptimal data during training to only the high and low diffusion times. To rigorously justify our approach, we first observe that robot action data exhibits a spectral power law. This induces two important properties on the optimal Diffusion Policy that we exploit: a global-to-local hierarchy and locality. We theoretically formalize this discussion using a simplified model. Our experiments validate Ambient Diffusion Policy on four types of suboptimal action data (noisy trajectories, sim-to-real gap, task mismatch, and large-scale data mixtures) across six tasks. The results show that it effectively learns from arbitrary sources of suboptimal data. Notably, it outperforms existing co-training baselines by up to 33% when scaled to Open X-Embodiment - a large dataset with heterogeneous data quality and unstructured distribution shifts. Overall, Ambient Diffusion Policy increases the utility of suboptimal demonstrations and expands the set of usable data sources in robotics.

Project website: [ambient-diffusion-policy.github.io](https://ambient-diffusion-policy.github.io/)

Please read the [paper](https://arxiv.org/abs/2606.12365) for more details.
