---
title: "Infilling Score: A Pretraining Data Detection Algorithm for Large Language Models"
collection: publications
permalink: /publication/infill_score
excerpt: ''
status: 'Published'
venue: 'ICLR 2025'
authors: 'Negin Raoof, Litu Rout, <strong> Giannis Daras</strong>, Sujay Sanghavi, Constantine Caramanis, Sanjay Shakkottai, Alexandros G. Dimakis'
paperurl: https://openreview.net/forum?id=9QPH1YQCMn
date: 2024-11-02
---


> In pretraining data detection, the goal is to detect whether a given sentence is in the dataset used for training a Large Language Model LLM). Recent methods (such as Min-K % and Min-K%++) reveal that most training corpora are likely contaminated with both sensitive content and evaluation benchmarks, leading to inflated test set performance. These methods sometimes fail to detect samples from the pretraining data, primarily because they depend on statistics composed of causal token likelihoods. We introduce Infilling Score, a new test-statistic based on non-causal token likelihoods. Infilling Score can be computed for autoregressive models without re-training using Bayes rule. A naive application of Bayes rule scales linearly with the vocabulary size. However, we propose a ratio test-statistic whose computation is invariant to vocabulary size. Empirically, our method achieves a significant accuracy gain over state-of-the-art methods including Min-K%, and Min-K%++ on the WikiMIA benchmark across seven models with different parameter sizes. Further, we achieve higher AUC compared to reference-free methods on the challenging MIMIR benchmark. Finally, we create a benchmark dataset consisting of recent data sources published after the release of Llama-3; this benchmark provides a statistical baseline to indicate potential corpora used for Llama-3 training.



Please read the [paper](https://openreview.net/forum?id=9QPH1YQCMn) for more details.
