---
title:  "Language Translation using Encoder Decorder"
mathjax: true
layout: post
categories: media
---


## Lists

### Table of contents :
1. troduction to seq-to-seq models.
2. encoder.
3. Decoder.
4. Code walk-through.
5. Evaluating performance on test data.
6. Conclusion.
7. References.


# 1- An introduction to Sequence-to-Sequence models :

## What is sequence-to-sequence learning?
Sequence-to-sequence learning (Seq2Seq) is about training models to convert sequences from one domain (e.g. sentences in English) to sequences in another domain (e.g. the same sentences translated to French).

"the cat sat on the mat" -> [Seq2Seq model] -> "le chat etait assis sur le tapis"
This can be used for machine translation or for free-from question answering (generating a natural language answer given a natural language question) -- in general, it is applicable any time you need to generate text.

There are multiple ways to handle this task, either using RNNs or using 1D convnets. Here we will focus on RNNs.


The job of encoder network is to understand the input sequence and create a smaller dimensional representation of it which is in turn forwarded to the decoder network that generates the output.

Input to the encoder may be an encoded sentence (in case of neural machine translation) or image features (in case of image captioning) or even sound waves (in case of speech recognition).

Some applications of Seq2Seq models are Neural machine translation, Image captioning, speech recognition, chat-bot, time-series forecasting e.t.c.


# 1. Neural Machine Translation

![English to Franch Translation](https://blog.keras.io/img/seq2seq/seq2seq-teacher-forcing.png)


# 2. Speech to text

![Speech to text](https://miro.medium.com/max/3932/1*nJNxFmJaHxyJTtVFkhGTlg.png)

# 3. Image captioning

![Image captioning](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/11/Model-of-Image-Caption-Generator-python-project.png)

