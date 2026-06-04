---
layout: page
title: Model Merging for Low-Resource ASR
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 2
category: lab
---

Speech foundation models (SFMs) such as Whisper underperform on low-resource domains like children's speech, where labeled data is scarce and acoustic-linguistic mismatch with the pretraining distribution is large. This work introduces Selective Attention (SA) Merge, a model merging method that combines task vectors from the self-attention matrices of multiple domain-finetuned checkpoints, rather than naively averaging entire models. By restricting the merge to attention parameters, SA Merge preserves the complementary specializations learned during finetuning while avoiding the interference that hurts full-model averaging. Combined with data augmentation, SA Merge produces a 14% relative Word Error Rate reduction and a state-of-the-art WER of 8.69 on the MyST child speech corpus for the Whisper-small model.


This work was presented at ICASSP 2025, and can be accessed <a href="https://doi.org/10.1109/ICASSP49660.2025.10887889"> here</a>


A journal extension of this work studies compositional domain adaptation: rather than training a separate model for each combination of distribution shifts (acoustic conditions, speaking style, speaker population), it asks whether the model updates induced by distinct supervision sources can be recombined to generalize to unseen intersections. Using child ASR as a case study, where age-related acoustics and speaking style jointly define a difficult low-resource setting, we propose a structured model merging framework that composes task-specific adaptations without retraining. To enable stable and interpretable composition, we introduce Headwise Selective Attention (HSA) Merge, which restricts parameter arithmetic to the salient attention heads where task-specific adaptations are concentrated. We further demonstrate robustness under acoustic mismatch, cross-corpus transfer, dialectal variation, and when source vectors are derived from synthetic or noisy data. Across Whisper model sizes, HSA Merge consistently outperforms single-source fine-tuning by relative WER of up to 20.6% on child ASR and 29.2% on cross-dialect transfer, indicating that key factors of variation in ASR models behave as partially separable components that structured attention-level merging can recombine.


This extension was published in Computer Speech & Language, and can be accessed <a href="https://www.sciencedirect.com/science/article/pii/S0885230826000756"> here</a>


The code can be accessed <a href="https://github.com/balaji1312/sa_merging"> here</a>, with the headwise extension available <a href="https://github.com/balaji1312/hsa_merge"> here</a>
