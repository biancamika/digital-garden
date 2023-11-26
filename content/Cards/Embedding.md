---
title: '"Embedding"'
---
## Reference
- **Source:** https://stable-diffusion-art.com/embedding/
- **Keywords:** [[Cards/permanent notes]]
	- #AI #computerscience 
- **Relevant Notes:** 
## Notes
- The result of [Textual Inversion](https://textual-inversion.github.io/): a method to define new keywords in a model ==without modifying it.==
- The method has gained attention because its capable of injecting new **styles** or **objects** to a model with as few as 3 -5 sample images.
	- The amazing thing about textual inversion is NOT the ability to add new styles or objects — other fine-tuning methods can do that as well or better. It is the fact that it can do so ==_without_ changing the model.==

### How Textual Inversion works
- First you define a **new** **keyword** that’s **not** in the model for the new object or style. That new keyword will get **tokenized** (that is represented by a number) just like any other keywords in the prompt.
- Each token is then converted to a unique **embedding vector** to be used by the model for image generation.
- Textual inversion finds the embedding vector of the new keyword that best represents the new style or object, without changing any part of the model. 
	- You can think of it as finding ==a way _within_ the language model to describe the new concept.==

![[Extras/Media/Images/Embedding Model.png]]
### How to use embeddings
