---
title: "Improving sparse transformer models for efficient self-attention"
collection: talks
type: "Talk"
permalink: /talks/spacy_irl
venue: "spaCyIRL"
date: 06/07/2019
location: "Berlin, Germany"
video: "https://www.youtube.com/embed/KwKr_e7xBQ4"
---


One disadvantage of using attention layers in a neural network architecture is that the memory and time complexity of the operation is quadratic. This talk tries to address the following question: "*Can we design attention layers with lower complexity that are able to discover all dependencies in the input?*".
The answer seems to be yes, by modeling the problem of introducing sparsity to the attention layer with Information Flow Graphs.


The contributions are the following: (i) a theoretical framework for designing new attention patterns is established, (ii) the importance of Full Information, the ability to discover any possible dependency in the input, is discussed, (iii) new attention patterns with Full Information are proposed, reducing the attention complexity to $O(n\sqrt n)$.
