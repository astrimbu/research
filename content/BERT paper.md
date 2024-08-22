---
title: BERT paper
aliases:
  - Bidirectional Encoder Representations from Transformers
tags:
  - 🖥️
---

https://arxiv.org/abs/1810.04805

Bidirectional  
Encoder  
Representations from  
Transformers

The paper titled "BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding" introduces a new language representation model called BERT (Bidirectional Encoder Representations from Transformers). The key innovation of BERT is its ability to pre-train deep bidirectional representations from unlabeled text by jointly conditioning on both left and right context in all layers. This approach contrasts with previous models that typically process text in a unidirectional manner.  

### Key Points:

1. **Model Design**: BERT is designed to pre-train using a bidirectional approach, enabling it to better understand context from both directions in text.
2. **Fine-Tuning**: After pre-training, BERT can be fine-tuned with a simple additional output layer to perform a variety of tasks, such as question answering and language inference, without needing substantial modifications to the architecture.
3. **Performance**: BERT achieves state-of-the-art results on eleven natural language processing tasks. Notable improvements include:
    - GLUE score of 80.5%, a 7.7% absolute improvement.
    - MultiNLI accuracy of 86.7%, a 4.6% absolute improvement.
    - SQuAD v1.1 question answering Test F1 score of 93.2, a 1.5 point absolute improvement.
    - SQuAD v2.0 Test F1 score of 83.1, a 5.1 point absolute improvement.

### Impact:

BERT's introduction has significantly advanced the field of natural language processing by providing a powerful, flexible, and empirically effective model for a wide range of language understanding tasks.

For further reading, you can access the full paper [here](https://arxiv.org/abs/1810.04805).
