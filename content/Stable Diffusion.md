---
title: Stable Diffusion
tags:
  - computer-science
  - computer-vision
  - ai
  - machine-learning
  - ai-art
---
#TODO:
- [ ] What is it
- [ ] What research enabled it
- [ ] 1.5 vs XL vs 3
- [ ] What else is out there (DALL-E, Midjourney)

Stable Diffusion (SD) is a text-to-image model developed by Stability AI.

**TL;DR:**  
- make static _(only easy step)_
- iteratively denoise static (n times)
	- guided by CLIP text encoder
		- pretrained on concepts
			- +attention mechanism
- return a representation of the trained concept

See also: [[AI Art]]