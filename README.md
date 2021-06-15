# Fine-tune with T5 & BERT

(retrieve from 21/03/15)

- Bi-directional Encoder from scratch using Trax
- Fine-tune with pre-trained BERT Loss
- Fine-tune with pre-trained T5 on SQuAD data

<br>

  ## Pre-processing

Data: Few example of  [C4](https://www.tensorflow.org/datasets/catalog/c4)  data and SQuAD

Tokenize : sentencepiece



<br>

  ## Bi-directional Encoder from scratch using Trax

Build Bi-directional Encoder from scratch using Trax



<img src="./encoder.png" alt="model" style="zoom:50%;" />

Model structure : 512 Embedding size, 6xEncoder, 8x multi head, using 0.1 dropout rate



positional encoding -> Masking -> Encoders -> LayerNorm -> Dense -> Softmax



Encoder detail :  LayerNorm -> Attention -> Dropout -> FFNN(2048->512)





