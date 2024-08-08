---
title: Stable Diffusion
aliases:
  - SD
---

[[Stable Diffusion]] (SD) is a text-to-image model developed by Stability AI / CompVis group.  

Stable Diffusion consists of 3 parts: the [variational autoencoder](https://en.wikipedia.org/wiki/Variational_autoencoder "Variational autoencoder") (VAE), [U-Net](https://en.wikipedia.org/wiki/U-Net "U-Net"), and an optional text encoder.  

- user provides text description
- **CLIP** text encoder converts text description into meaningful vector representation
	- **Contrastive Language-Image Pre-training** is a model developed by OpenAI  
	- Encoder converts text --> vector rep *(captures semantic meaning)*

---

tags: [[Computer science]] - [[AI]]