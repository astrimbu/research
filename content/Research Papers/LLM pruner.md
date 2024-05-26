---
title: LLM-Pruner On the Structural Pruning of Large Language Models
tags: 
  - computer-science
  - language
  - 2023
---

https://arxiv.org/pdf/2305.11627.pdf

The paper "LLM-Pruner: On the Structural Pruning of Large Language Models" introduces LLM-Pruner, a framework for compressing large language models (LLMs) while retaining their general-purpose capabilities. The key innovation of LLM-Pruner is structural pruning, which identifies and removes non-critical parts of the model based on gradient information. This method aims to minimize the need for the original training dataset and allows the pruned models to retain most of their functionality with significantly fewer parameters.

### Key Points:

1. **Challenges Addressed**:
    - **Task-Agnostic Compression**: The goal is to compress LLMs without relying on specific tasks, ensuring the models maintain their ability to perform a variety of tasks.
    - **Reduced Data Dependency**: Traditional compression methods often require extensive retraining on the original dataset, which is impractical due to the dataset's size and potential proprietary restrictions.

2. **LLM-Pruner Methodology**:
    - **Dependency Detection**: The method starts by identifying interdependent structures within the model to ensure that pruning does not disrupt the model's functionality.
    - **Importance Estimation**: Once the dependent structures are identified, the importance of each group is estimated using first-order and second-order gradient information.
    - **Fast Recovery with Low-Rank Approximation**: The pruned model undergoes a quick post-training phase using limited data, facilitated by low-rank approximation techniques to optimize only a small subset of parameters.

3. **Evaluation and Results**:
    - **Models Tested**: LLM-Pruner was tested on three models: LLaMA-7B, Vicuna-7B, and ChatGLM-6B.
    - **Performance Metrics**: The models were evaluated on tasks including zero-shot classification and language generation using nine different datasets.
    - **Efficiency**: The pruned models retained up to 94.97% of the original model's performance, demonstrating that the LLM-Pruner can effectively compress models while maintaining their capabilities.

4. **Advantages**:
    - **Task-Agnostic**: The method allows LLMs to retain their general-purpose nature after compression.
    - **Minimal Training Data**: Only 50K publicly available samples are needed for post-training, reducing the data acquisition burden.
    - **Quick Compression**: The entire compression process can be completed in just three hours on a single GPU.

### Conclusion:
LLM-Pruner presents a significant advancement in the compression of large language models. By focusing on structural pruning and minimizing reliance on the original training data, it offers a practical and efficient solution for reducing the size of LLMs while preserving their diverse capabilities. This approach not only makes LLM deployment more feasible but also opens up new possibilities for using these models in resource-constrained environments.

For more details, you can access the full paper [here](https://arxiv.org/pdf/2305.11627.pdf).