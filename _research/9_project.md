---
layout: page
title: Model Merging for Low-Resource ASR
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 1
category: lab
---

Speech foundation models (SFMs) such as Whisper underperform on low-resource domains like children's speech, where labeled data is scarce and acoustic-linguistic mismatch with the pretraining distribution is large. This work introduces Selective Attention (SA) Merge, a model merging method that combines task vectors from the self-attention matrices of multiple domain-finetuned checkpoints, rather than naively averaging entire models. By restricting the merge to attention parameters, SA Merge preserves the complementary specializations learned during finetuning while avoiding the interference that hurts full-model averaging. Combined with data augmentation, SA Merge produces a 14% relative Word Error Rate reduction and a state-of-the-art WER of 8.69 on the MyST child speech corpus for the Whisper-small model.


This work was presented at ICASSP 2025, and can be accessed <a href="https://doi.org/10.1109/ICASSP49660.2025.10887889"> here</a>


The code can be accessed <a href="https://github.com/balaji1312/sa_merging"> here</a>
