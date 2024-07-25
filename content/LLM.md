---
title: Large Language Model
aliases:
  - large language model
---

What's a machine learning model?  
> An object/file that has been conditioned by an algorithm to learn specific patterns in datasets  

What's an LLM?  
> A machine learning model designed to understand and generate human language  
> Trained on vast amounts of text data  

Today's most powerful open-weights model is Meta's Llama3.1  

LLM's are made up of two files, `parameters` and `run.c`  

- `parameters` contains the weights of the language model. For example, Llama3:8b has a parameter size of 8 billion, so the `parameters` file will be 16GB (you need two bytes (float16) to store each parameter).  

- `run.c` contains ~500 lines of C code to implement the NN architecture that uses the parameters to run the model  

---

How to train an LLM from scratch:  

1. Pretraining (base model)  
	1. Download ~10TB text
	2. Buy cluster of ~6,000 GPUs
	3. Lossy compress text into a neural network (~$2M, ~12 days)
	4. Obtain `base model`

2. Finetuning (assistant model)  
	1. Write labeling instructions
	2. Hire people to write quality Q&A responses (and/or comparisons ([[RLHF]]))
	3. "Finetune" base model on this data (~1 day)
	4. Obtain `assistant model`
	5. Run evaluations
	6. Deploy
	7. Monitor, collect misbehaviors, go to step 1

---

Todo: expand on the following:
- [ ] Closed-source models
- [ ] Llama3, 3.1
- [ ] OpenWebUI
- [ ] Ollama

---

tags: [[Computer Science]] - [[Language]] - [[ML]] - [[AI]]