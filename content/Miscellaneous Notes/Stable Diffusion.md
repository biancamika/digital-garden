---
title: “Stable Diffusion"
---
## Reference
- **Source:** https://www.youtube.com/watch?v=dMkiOex_cKU&t=328s
- **Keywords:** [[Cards/permanent notes]]
	- #AI #art #computerscience 
- **Relevant Notes:** 
	- [[Cards/Prompt engineering|Prompt engineering]]
## Notes
- Stable Diffusion is a [[Cards/Latent Diffusion Model]] for generating AI images
- On Models
	- The official models released by Stability AI and their partners are called **base models**. Some examples of base models are Stable Diffusion [1.4](https://stable-diffusion-art.com/models/#Stable_diffusion_v14), [1.5](https://stable-diffusion-art.com/models/#Stable_diffusion_v15), [2.0](https://stable-diffusion-art.com/how-to-run-stable-diffusion-2-0/), and [2.1](https://stable-diffusion-art.com/install-stable-diffusion-2-1/).
		- Stick with the **base models** if you are starting out.
	- [Custom models](https://stable-diffusion-art.com/models/) are trained from the base models. Currently, most of the models are trained from v1.4 or v1.5. They are trained with additional data for generating images of particular styles or objects.
	- There are two ways of training models: [[Dreambooth]] and [[Cards/Embedding]]
- [[Cards/LoRa Models]] make image generation more efficient by encapsulating training parameters into one model keyword (e.g. <lora:lydia-08:1>) 
	- You can start making the dataset of your first LoRa model by generating images from SD
	- This is how you can start working towards [datasets as imagination](https://joinreboot.org/p/artist-datasets)
- [[Cards/ControlNet]] gives you finetuning power over your images
- [[Variable Auto Encoder]] is a file you use in addition to your Stable Diffusion checkpoint models to get more vibrant colors and crisper images. 
	- They hep with improving hands and faces.
- Notes
	- You may have to subscribe to Pencilcase or Rundiffusion for more memory...
	- For resources: go to https://civitai.com/ for models to use. You can also check out the prompts used for images here
	- For Midjourney style, use this model: https://openjourney.art/
	- Full courses: https://prompthero.com/academy/