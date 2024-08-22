---
title: ControlNet paper
aliases:
  - Adding Conditional Control to Text-to-Image Diffusion Models
tags:
  - 🖥️
---

https://arxiv.org/abs/2302.05543

The paper "Adding Conditional Control to Text-to-Image Diffusion Models" introduces ControlNet, a neural network architecture designed to add spatial conditioning controls to large, pretrained text-to-image diffusion models.

### Summary:

- **ControlNet Architecture**:
    
    - ControlNet leverages existing large diffusion models without altering them.
    - It uses deep and robust encoding layers, pretrained with billions of images, as a backbone.
    - The network employs "zero convolutions" (zero-initialized convolution layers) to progressively grow parameters from zero, ensuring no harmful noise impacts fine-tuning.

- **Conditional Controls**:
    
    - Various types of conditional controls are tested, such as edges, depth, segmentation, and human pose.
    - These controls can be applied using single or multiple conditions, with or without prompts.  

- **Training and Robustness**:
    
    - The training of ControlNets is shown to be robust with both small (<50k) and large (>1m) datasets.
    - Extensive results indicate that ControlNet can enhance the control of image diffusion models, potentially facilitating a wide range of applications.

For further details, you can view the full paper [here](https://arxiv.org/abs/2302.05543).
