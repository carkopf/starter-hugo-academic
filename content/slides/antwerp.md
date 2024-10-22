
---
title: Two constraints on the neuroscience of content
summary: I describe two non-obvious theoretical constraints on any attempt to decode propositional attitudes from brain data. 
authors: []
categories: []
date: '2019-02-05'
slides: true
theme: 'white'
highlight_style: dracula

---

## Two constraints on the neuroscience of content

Charles Rathkopf

Center for Philosophical Psychology

March 21st, 2024

---

## What are the theoretical limits on mind-reading?

1. The relevant data is too hard to acquire 
2. The relevant data is too hard to interpret
3. The relevant data is not (exclusively) located in the brain

{{% speaker_note %}}
- here I focus on BELIEF
- If there are no constraints, then I can work out on the basis of brain data any and all your beliefs
{{% /speaker_note %}}

---

### What is mind-reading?

Decoding mental content from brain data such that: 

1. No conventional symbols
2. Driven by neural data


{{% speaker_note %}}
- Can't rely on normal means of communication
- Communication has a productive side and a receptive side.
{{% /speaker_note %}}

---
## No conventional symbols

Rule out the intentional production of conventional symbols like words.

1. Thought-to-text devices 
2. fNIR for ALS patients 

---

## Driven by neural data

1. Social cognition takes behavior as input 
2. Mind-reading takes exclusively neural data as input
    - e.g. predictive algorithm cannot take behavioral response latency as input

{{% speaker_note %}}
- Do we need another condition to say what mindreading really is?
- I think we might, but to see it we need to look at an experiment. 
{{% /speaker_note %}}

---

## Typical decoding experiment

1. Each measurement site in the brain is represented as one dimension in a high-dimensional space 
2. ML used to associate each point with some property of the experimental condition in which it was elicited
3. Typically stimulus classification, sometimes reconstruction

---

## From stimulus prediction to attitude ascription

1. Speeded one-back repetition detection task.  
2. Algorithm predicts house/face & correct/incorrect from brain data
3. Where t is a correct house trial, we infer "S believes that the image on trial t was a house"

{{% speaker_note %}}
- Some rational reconstruction here. 
- Maybe subject believes that the experiment is about illusions, so she believes the opposite of what her perceptual evidence suggests.
- Degree of RR inversely proportional to strangeness of thought experiment 
{{% /speaker_note %}}

---

## Too much rational reconstruction?

1. Images of gesture
2. Dutch hand-ear gesture 
3. Infer: S believes that the person in the photo likes the food

{{% speaker_note %}}
- Experimenter contributes too much. No longer "pure decoding."  
- Solution: make the computer do this work. Then you can control exactly which factors are allowed to influence the propositional attitude ascription. 
- But how do you get computer to print out propositions that describe what is going on in the subject's mind? 
{{% /speaker_note %}}

---

## Decoding propositional content

- Tang et al. (2023) reconstructs continuous natural langauge from both perceived and imagined speech 
- Relies on neural representations of semantic meaning, rather than acoustic or phonetic information
- Decoder trained within-subject on 16 hours of fMRI data, with narrative audio

{{% speaker_note %}}
- The Tang et al study is not about belief per se. 
- But also not just about perception. One condition is perceptual, and another one is imagined speech.
- Subjects read stories, then imagine telling them. 
- Decoder was not as good as in perception condition, but well above chance.
- Not surprising since decoder was trained on perceived speech.
{{% /speaker_note %}}

---

## Results from perceived speech experiment

![Decoded Language from Tang et al. (2023)](/antwerp_images/decoded_language.png)
from Tang et al. (2023)


---
## Rational reconstruction in a computer program

![Experimental pipeline](/antwerp_images/pipeline.png)
from Tang et al. (2023)

{{% speaker_note %}}
- LLM used twice
- First to create embeddings for each word
- Encoder maps brain data to word sequences, but you can use it to rank the probability that a given word sequence produced a given brain image. You just need to provide a shortish list of possible word sequences to run through the model. 
- LLM used for this as well. 
{{% /speaker_note %}}

---

## Need for generative models

1. LLM generates new language based on plausibility
2. This is a form of rational reconstruction
3. Conjecture: some form of rational reconstruction will always be necessary

{{% speaker_note %}}
- We need to run a "generative model" to get to attitude ascription, regardless of whether it is a person or a program doing the ascription. 
- This brings us to philosophical theories of belief. Roughly the idea is that "superficialist theories" are committed to this conjecture, while representationalist theories are not.    
{{% /speaker_note %}}

---

## Deep theories of belief 

```
1. Representationalist

    - Beliefs are relations to structured mental 
    representations 
```
```
2. Psychofunctionalist 

    - Representations are explicitly stored in the brain 
    - Yes-or-no phenomenon
    - To be discovered by mind/brain sciences 
```
{{% speaker_note %}}
- On this view, as long as we have instruments that give access to the relevant data, and enough inferential machinery, neuroscience should eventually be able to say in each case whether someone believes that P, or does not.
{{% /speaker_note %}}

---

## Superficialist theories of belief

```
Whether an agent has the belief that P depends only on 
whether their patterns of actual and potential behavior 
come sufficiently close to matching a stereotype of 
rational action for agents with the belief that P
```
{{% speaker_note %}}
 - Mental representations are essential to belief only to the extent that they ground such a pattern of behavior 
- Includes dispositionalist and interpretationist views  
- Schwitzgebel, Ryle, Lewis, Davidson, Dennett, Frances Egan
{{% /speaker_note %}}

---
### Superficialists are committed to the conjecture

1. Stereotypes of rational action are essential to belief
2. Stereotypes depend on population-level facts about behavior
3. Therefore, belief-determining facts not (only) in the brain
4. Therefore, no empirical discovery will relieve us of the need for rational reconstruction. 

{{% speaker_note %}}
This is the first constraint from my title. If you're superficialist, you have to deny that pure decoding is possible, where "pure" decoding means no rational reconstruction.
{{% /speaker_note %}}

---

## Trumping cases
```
1. Behavioral data, including biographical information, 
support the claim that the subject believes that P, but

2. Brain data supports the claim that the subject 
believes that ~P, and 

3. The brain data constitutes stronger evidence 
about what the subject really believes than the 
behavioral evidence
```

{{% speaker_note %}}
- These cases are impossible for the superficialist 
- This is the second constraint from my title
- Patterns of activation in the brain might cause the behavioral dispositions to match a given stereotype better or worse, but this relation is causal rather than logical. 
{{% /speaker_note %}}

---
## Have we made progress? 

1. Added empirical commitment to superficialist theory of belief
2. Sharpened the distinction between the deep and superficialist views
    - worry: Mandelbaum & Schwitzgebel talking past each other
    - Trumping cases show that disambiguation of "belief" does not dissolve the disagreement

{{% speaker_note %}}
- consider debate between Mandelbaum and Quilty-Dunn on the one side, and Schwitzgebel on the other. 
- Worry that they talk past each other because there are two kinds of belief
- A superficial kind which we will retain no matter what neuroscience discovers, and another, superficialist kind which may diverge from our folk habits of attitude ascription 
- We can have both, you might think. Mandelbaum can give us reasons to think that mental representations that cause behavior are propositional, and he wants to call them belief. Schwitzgebel thinks lots of what we will insist on calling belief is probably not so clearly defined in the brain. 
- So they are talking past. 
- But now consider trumping cases. This reveals that they are not merely talking past each other. With respect to trumping, the views are in direct competition.  
{{% /speaker_note %}}

---

Thanks for your attention!

---









