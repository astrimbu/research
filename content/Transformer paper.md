---
title: Transformer paper
aliases:
  - Attention Is All You Need
tags:
  - 🖥️
---

https://arxiv.org/abs/1706.03762  

The paper "Attention Is All You Need" by Ashish Vaswani et al. introduces a new neural network architecture called the Transformer, which relies solely on attention mechanisms, foregoing [[RNN|recurrence]] and [[CNN|convolutions]] entirely. This architecture aims to address limitations in previous models that depend on complex recurrent or convolutional networks for sequence transduction tasks such as machine translation.  

### Key Points:

1. **Transformer Model Architecture**:
    - The Transformer model uses an encoder-decoder structure, where both the encoder and decoder are composed of multiple layers of self-attention mechanisms and fully connected feed-forward networks.
    - The encoder consists of a stack of identical layers, each containing a multi-head self-attention mechanism and a position-wise fully connected feed-forward network.
    - The decoder is similarly composed but includes an additional sub-layer that performs multi-head attention over the encoder's output.

2. **Self-Attention Mechanism**:
    - Self-attention, or intra-attention, allows the model to weigh the importance of different positions within the same sequence.
    - The attention mechanism used is "Scaled Dot-Product Attention," which scales the dot products of the input vectors and applies a softmax function to obtain attention weights.
    - Multi-head attention extends this mechanism by allowing the model to focus on different parts of the sequence simultaneously using multiple attention heads.

3. **Positional Encoding**:
    - Since the model does not use recurrence or convolution, it incorporates positional encodings to maintain information about the order of the sequence.
    - These encodings are added to the input embeddings and are generated using sine and cosine functions of different frequencies.

4. **Training and Performance**:
    - The Transformer can be trained more efficiently and in a more parallelized manner compared to recurrent models.
    - On the WMT 2014 English-to-German and English-to-French translation tasks, the Transformer achieved state-of-the-art performance, with BLEU scores of 28.4 and 41.8, respectively.
    - The model's training efficiency is highlighted by its ability to train to these high levels of accuracy in significantly less time than previous models.

5. **Advantages and Future Work**:
    - The Transformer offers greater parallelization and efficiency in training due to its reliance on self-attention.
    - It generalizes well to other tasks, such as English constituency parsing, demonstrating its versatility.
    - Future research will explore extending the Transformer to other modalities beyond text and improving its handling of long sequences through restricted attention mechanisms.

### Conclusion:
The introduction of the Transformer model marks a significant advancement in sequence transduction models by utilizing attention mechanisms alone. This approach not only improves performance but also enhances training efficiency, paving the way for further innovations in natural language processing and beyond.  
