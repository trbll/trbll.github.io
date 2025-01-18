---
layout: posts
title: From Brain State Prediction to Memory Engineering
excerpt: "Recent breakthroughs in brain activity modeling hint at a future where memories become malleable digital constructs."
tags: [thought]
date: 2025-01-18 10:30:00
---

## From Brain State Prediction to Memory Engineering

> "The past is never dead. It's not even past."
>
> **William Faulkner**, *Requiem for a Nun* (1950)

A recent paper from researchers at the University of Sydney demonstrates something remarkable: **AI can predict brain states**[^1]. Using the transformer architecture—the same technology powering modern AI language models—researchers successfully predicted ~5 seconds of brain activity from ~20 seconds of recorded data. 

The researchers achieved this using fMRI data representing activity across 379 brain regions. Impressively, their predictions maintained functional connectivity patterns—the complex web of relationships between different brain areas. In other words, the predicted brain states weren't just random activity; they preserved the fundamental organization of brain function.

From 30 fMRI scans, their model could accurately predict the next 7 consecutive brain states. How accurately? The first predicted time point/state following the inputs had **a correlation of 0.997 with the ground truth fMRI data.** And the first 5 predicted states had a correlation of greater than 0.85! 

Extrapolating: <u>we now have a model that can predict **into the future** what the brain will do next.</u>

### Parallels to Language Models

The results might seem modest at first glance and this extrapolation might seem extreme. But consider the trajectory of language models. GPT-3 completed the text from some user-provided context and input prompt. 

#### Example 1: [Movie to Emoji Generation](https://andrewmayne.com/2020/06/24/open-ai-alchemy-emoji-storytelling/)

**Input:**

```
Back to Future: 👨👴🚗🕒
Batman: 🤵🦇
Transformers:  🚗🤖
Star Wars: 
```

**Output:**
```
🚀🏰🚀
```

#### Example 2: [First-Person to Third-Person Writing](https://brookechan.notion.site/1st-3rd-Person-Writing-ba3be8267da042498c5cc7430558c2a8)

**Input:**

```
in: i started the business in 2010 we sell gift boxes with chocolates and other things   
out: The business was founded in 2010, and they sell gift boxes with chocolates and other items.

in: we don't have any investors   
out: The company has taken no outside funding.

in: our only major risk is our supplier who we depend on for 90% of our stock   
out: The company's main challenge is its dependence on a single supplier for 90 percent of its stock.
 
in: We have a lot of loyal customers and are growing rapidly   
out: The company has a lot of loyal customers and is growing rapidly.   

in: we don't use social media for marketing   
out: The company doesn't use social media for marketing.   
 
in: i am currently in the process of opening up a new store   
out: 
```

**Output:**
```
The company is currently in the process of opening up a new store.
```

### Trajectory of Impending Improvements

The brain study reminds me of GPT-3. In the same way that we provided some context and examples to GPT-3 with our input prompt, the 20 seconds of fMRI data is providing context and examples to the brain state prediction model. It then stands to reason that the improvements we have seen in LLMs since GPT-3 will be seen in brain state prediction. Not only is this logical from the standpoint of continous technology advancement (we have nowhere to progress but forward), but much of the groundwork required for these improvements have already been laid. 

Soon then we should see analogous improvements in brain state prediction along the lines of:
- **Increased input length:** longer fMRI history provided as contextual input to the model. 
- **Increased output length:** more accurately predicted states / more time predicted into the future.
- **Increased model strength and performance** at similar or fewer model parameters.
- **Faster inference time:** more states accurately predicted per fixed amount of time and compute.
- **Test-time compute (TTC):** reasoning-like search behavior that leads to more accurate predictions.
- **Thanks to TTC:** an abundance of better, increasingly generalized, synthetic data that can be used as training data for future models.
- **Thanks to improved training data:** stronger brain prediction models that can be (1) distilled down into (slightly weaker but) smaller and faster versions of themselves or (2) used to to generate even more and better synthetic data via TTC.
- **Takeoff:** the cycle and improvements repeat and continue.

Just as early language models learned to predict the next word in a sequence, we can now predict the next state in a sequence of brain activity. Just as language models progressed from simple prediction to understanding context, generating coherent long-form content, and engaging in complex reasoning, brain state prediction could evolve from brief moments to extended sequences of neural activity. I myself feel convinced about this and there is even more evidence to support it.

### Parallels to Video/World Models

### Free Will?

Just how far into the future will such models be able to accurately predict? If these models scale as I've just described, is predicting a minute of brain activity into the future possible? What about an hour? A day? 

What are the implications of free will then?


This breakthrough hints at a profound possibility: if we can predict and generate brain states that maintain neural organization, could we eventually reconstruct, enhance, or even create experiences at the neural level?

## The Memory Engineering Horizon

Imagine a neural interface that could read your brain's activity patterns and, combined with advanced AI, allow you to:

- Relive memories with enhanced clarity, as AI fills in the gaps in your recollection
- Adjust the emotional tone of remembered experiences
- Share processed, encoded memories with others
- Preserve personality patterns for future interaction
- Process and reshape traumatic memories in a controlled environment

These aren't just science fiction concepts anymore. The technical foundation - predicting and generating coherent brain states - is already being laid.

## Beyond Simple Recall

The implications extend far beyond just better memory recall. When memories become editable digital constructs, we enter uncharted territory:

- How does optimizing or enhancing memories affect our sense of self?
- What happens to personal identity when memories can be shared or experienced collectively?
- Could we develop "memory engineering" as a therapeutic tool?
- What are the ethics of modifying or sharing intimate neural experiences?

The researchers focused on immediate medical applications - reducing scan times, predicting seizures, advancing brain-computer interfaces. But they've demonstrated something more fundamental: the mathematical frameworks we use to model language and thought can also model physical brain states.

## The Road Ahead

We're still far from full memory manipulation. Current prediction windows are short, error accumulation remains a challenge, and we're working with relatively coarse fMRI data. But consider:

- Higher resolution brain interfaces are in development
- AI architectures grow more sophisticated by the month
- Our understanding of neural organization deepens constantly
- Quantum computing looms on the horizon

The question isn't if we'll achieve this level of neural engineering, but when - and more importantly, how we'll handle it when we do.

> "The future is already here – it's just not evenly distributed."
>
> **William Gibson**

As we stand at the threshold of this technology, we have a unique opportunity to shape its development. The technical foundations are being laid. The ethical frameworks need to catch up.

What kind of future do we want to build when memories become malleable?

[^1]: Sun, Y., Cabezas, M., Lee, J., Wang, C., Zhang, W., Calamante, F., & Lv, J. (2024). "Predicting Human Brain States with Transformer." <a href="https://arxiv.org/abs/2412.19814" target="_blank">arXiv:2412.19814</a>