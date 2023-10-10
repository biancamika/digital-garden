---
title: "Prompt engineering"
---
## Notes
### General syntax
- **Negative prompts:** used to describe what you don't want to see in the image. 
	- The AI sometimes ignores parts of the negative prompt, especially if the prompt and negative prompt contain very similar terms. 
	- In other cases, the negative prompt has big impact on the composition of the image.

```
Deformed, blurry, bad anatomy, disfigured, poorly drawn face, mutation, mutated, extra limb, ugly, poorly drawn hands, missing limb, blurry, floating limbs, disconnected limbs, malformed hands, blur, out of focus, long neck, long body, mutated hands and fingers, out of frame
```

### EasyDiffusion
- Append a word or phrase with `-` or `+`, or a weight between `0` and `2` (`1` is default), to decrease or increase the importance of that word/phrase in the generated image. For e.g. `man picking apricots+`
	- You can assign weights to multiple words by using parentheses. For e.g. `a man (picking apricots)1.5` or `a man (picking apricots)++`
	- You can add more `+` or `-` symbols to increase/decrease the weight further. For e.g. `apricot++` has more importance than `apricot+`, and `apricot--` has less importance than `apricot-`. There's no limit to how many `+` or `-` symbols you can use.
- You can also use a number to assign an exact weight to a word/phrase:
	- A weight between `0` and `1.0` reduces the importance of the token. For e.g. `(apricots)0.5` reduces the importance of apricots to half.
	- A weight between `1.0` and `2` increases the importance of the token. For e.g. `(apricots)1.5` increases the importance of apricots by 1.5 times.
### Midjourney
#### Types of Styles
![[Extras/Media/Images/Styles in Midjourney.png]]

- Design/genre
- Artist name
- Rendering/lighting

#### Stylize the output
```
--s <some number>
```


