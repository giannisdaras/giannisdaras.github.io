---
title: 'Parallel dataset construction for BERT pretraining in tensorflow 2'
date: 19/08/2019
permalink: /posts/bert_pretraining_parallel_data/
tags:
  - bert
  - transformers
  - tensorflow
---

Transformer inspired models such as [BERT](https://arxiv.org/abs/1810.04805), [XLNET](https://arxiv.org/abs/1906.08237) or [RoBERTa](https://ai.facebook.com/blog/roberta-an-optimized-method-for-pretraining-self-supervised-nlp-systems/) require
massive data for their unsupervised pre-training.

A common practice in [Tensorflow](https://www.tensorflow.org/) is to store large datasets in
TFRecord files, an efficient binary storage format. TFRecord files integrate
seamlessly with the data import and preprocessing functionality in Tensorflow.

When it comes to BERT pretraining, Google provides a [script](https://github.com/google-research/bert/blob/master/create_pretraining_data.py)
in the official Tensorflow implementation for creation of TFRecord files.

I am truly thankful for this script, because it does the hard work for us.
However, there are two issues I would like to address with this post: (i) it's
not Tensorflow 2 compatible, (ii) it doesn't have data parallelism.

Issue (i) can be resolved easily by replacing `tf.gfile.GFile` with
`tf.io.gfile.GFile`, `tf.gfile.Glob` with `tf.io.gfile.glob` and removing
`tf.logging` as it is replaced in Tensorflow 2 with [abseil](https://github.com/abseil/abseil-py).
Those changes can be easily made by hand or you could also try the automatic conversion script provided
by Google as explained [here](https://www.tensorflow.org/beta/guide/upgrade).

Issue (ii) regards data parallelism and it is crucial for large datasets
because tokenization can take a lot of time if it is performed on a single
cpu. In order to tackle this problem, we are using the [multiprocessing](https://docs.python.org/2/library/multiprocessing.html#module-multiprocessing)
python library and specifically the `Pool` class.


We change the API of the `create_training_instances` function; the new function takes a single
input file and create instances only for this file. This way, we can call this function
using `Pool` class on multiple cpus with different data each time and enable
data parallelism in our code.

The same logic applies to `write_instances_to_example_files` as well. Instead of
taking multiple output files, it takes a single output file and the instances that
will be written to this single file. Actually, we also modify `create_training_instances` in order to call
directly `write_instances_to_example_files` after the instances creation for
increased speed-up.

A version of this code can be found in this [gist](https://gist.github.com/giannisdaras/c1d6c08f52c0b5b7d6301fb6e1986a44).

Thanks for reading :)  
