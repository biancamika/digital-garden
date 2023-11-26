---
title: '"LoRa Models"'
---
## Reference
- **Source:** https://civitai.com/models/22530
- **Keywords:** [[Cards/permanent notes]]
- **Relevant Notes:** 
	- [[Miscellaneous Notes/Stable Diffusion|Stable Diffusion]]
## Notes
- **LoRa (Low Rank Adaptation)** is a new technique for fine-tuning deep learning models. It works by ==reducing the number of trainable parameters== and enables efficient task switching. 
- Can be trained and used for: characters/people, artstyles, poses/concepts, etc.
- Can take a LONG time to train models!

### How to make a LoRa
#### Making the dataset
- A dataset is (for us) a collection of **images** and their **descriptions**, where ==each pair has the same filename== (eg. "1.png" and "1.txt"), and ==they all have something in common which you want the AI to learn.== 
- The quality of your dataset is essential: You want your images to have at least ==2 examples== of: poses, angles, backgrounds, clothes, etc. 
	- If all your images are face close-ups for example, your Lora will have a hard time generating full body shots (but it's still possible!), unless you add a couple examples of those. 
- You can train a mediocre Lora with a bare minimum of 5 images, but I recommend ==20 or more, and up to 1000.==
- As for the descriptions, for general images you want ==short and detailed sentences== such as "_full body photograph of a woman with blonde hair sitting on a chair_".
	- This is how tags work in your dataset: You need to be detailed, as the Lora will reference what's going on by using the base model you use for training. 
		- Anything you **don't** include in your tags will **become part of your Lora**. This is because the Lora absorbs details that can't be described easily with words, such as faces and accessories. 
	- Knowing this you can let those details be absorbed into an **activation tag**, which is a ==unique word or phrase== that goes at the start of every text file, and which makes your Lora ==easy to prompt.==

1. Setup
2. Scrape images
3. Curate your images (remove duplicates)
4. Tag your images
5. Curate your tags
