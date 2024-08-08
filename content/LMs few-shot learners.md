---
title: LMs few-shot learners
aliases:
  - Language Models are Few-Shot Learners
tags:
  - 🖥️
---

https://arxiv.org/abs/2005.14165

The paper "Language Models are Few-Shot Learners" by Tom B. Brown et al. introduces GPT-3, an autoregressive language model with 175 billion parameters. This model demonstrates significant improvements in task-agnostic few-shot performance, suggesting that scaling up language models can enable them to perform a wide range of language tasks with minimal task-specific training.

### Key Points:

1. **Model Overview**:
    - GPT-3 is a transformer-based autoregressive language model with 175 billion parameters, which is 10 times larger than its predecessor, GPT-2.
    - The model is trained on a diverse dataset that includes Common Crawl, WebText, books, and Wikipedia.

2. **Few-Shot Learning**:
    - Unlike traditional models that require fine-tuning on large task-specific datasets, GPT-3 can perform various tasks by using a few examples provided at inference time (few-shot learning).
    - The model also supports zero-shot (no examples) and one-shot (one example) learning scenarios.

3. **Performance**:
    - GPT-3 achieves state-of-the-art performance in few-shot settings on many NLP tasks, including language modeling, translation, question answering, and cloze tasks.
    - For some tasks, GPT-3's few-shot performance is competitive with, or even surpasses, fine-tuned models despite not using task-specific training.

4. **In-Context Learning**:
    - GPT-3 uses in-context learning, where it leverages the context provided in the input text to understand and perform tasks.
    - Larger models like GPT-3 show improved ability to learn from context, making them more efficient at in-context learning.

5. **Task Performance Examples**:
    - GPT-3 achieved strong performance on CoQA with F1 scores of 81.5 (zero-shot), 84.0 (one-shot), and 85.0 (few-shot).
    - On TriviaQA, it achieved accuracies of 64.3% (zero-shot), 68.0% (one-shot), and 71.2% (few-shot).

6. **Limitations**:
    - GPT-3 struggles with certain tasks, such as natural language inference (e.g., ANLI) and some reading comprehension tasks (e.g., RACE, QuAC).
    - Data contamination is a concern, as training on large web corpora can inadvertently include content from test datasets.

7. **Broader Impacts**:
    - The paper discusses potential biases and societal impacts, emphasizing the need for careful consideration in the deployment of such powerful models.

### Conclusion:
GPT-3's ability to perform a wide range of tasks with minimal task-specific training demonstrates the potential of scaling up language models for achieving better generalization and versatility. Its performance in few-shot learning settings highlights significant advancements in NLP, though there are still areas for improvement and ethical considerations to address.

For more details, you can access the full paper [here](https://arxiv.org/abs/2005.14165).

---

tags: [[Computer science]] - [[Research]] - [[Language]]