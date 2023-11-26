---
title: '"Latent Diffusion Model"'
---
## Reference
- **Source:** 
- **Keywords:** [[Cards/permanent notes]]
	- #AI #art #computerscience 
- **Relevant Notes:** 
	- [[Miscellaneous Notes/Stable Diffusion|Stable Diffusion]]
	- [[Cards/Prompt engineering|Prompt engineering]]
## Notes
- A Latent Diffusion Model is a type of generative model used in machine learning and artificial intelligence. 
- It's specifically designed for modeling and generating complex, high-dimensional data like images, text, and more. 
	- The term "latent" refers to the fact that the model ==captures hidden or latent representations== within the data.

### Key Components and Concepts
- **Diffusion Process:** The term "diffusion" in Latent Diffusion Models refers to a probabilistic process. 
	- It models how data evolves or changes over time. 
	- Essentially, it describes the ==transformation of an initial data point== (e.g., a random noise vector) into the ==observed data== (e.g., an image) through a series of steps. 
	- Each step is guided by a probability distribution, and the data becomes more complex and realistic as the diffusion process progresses.
- **Latent Space:** The model learns a latent space, which is an ==abstract representation of the data that captures its underlying structure and features.== 
	- This latent space is a lower-dimensional space that encodes useful information about the data. 
	- It's often compared to a compressed representation of the data, where similar data points in the original high-dimensional space are close together in the latent space.
- **Invertible Model:** In Latent Diffusion Models, the transformations in the diffusion process are invertible. This means ==you can move both forward and backward in the process. ==
	- Given an observed data point, you can sample from the latent space and generate a similar data point by reversing the diffusion process. This property is crucial for generating new data samples.
- **Generative Modeling:** Latent Diffusion Models are generative models, meaning ==they can generate new data samples that resemble the training data. ==
	- To generate a new sample, you start with a random noise vector in the latent space and apply the inverse diffusion process to generate data in the high-dimensional space. 
	- These generated samples can be used for various applications, such as image synthesis, data denoising, or data completion.
- **Training:** Training a Latent Diffusion Model involves learning the parameters of the model, including the parameters that define the diffusion process and the mapping between the latent space and the high-dimensional data space. 
	- Training typically involves optimizing a likelihood function that measures how well the model can reproduce the training data.
