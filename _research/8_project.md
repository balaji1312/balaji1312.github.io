---
layout: page
title: Improving ASR for Child Speech
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 2
category: lab
---

This project presents a novel framework for unsupervised domain adaptation of speech foundation models to low resource domains. Speech foundation models finetuned on certain domains, such as LibriSpeech (adult read speech), behave poorly on other domains (child or noisy speech). One solution could be collecting as much labelled data as possible for joint finetuning on various domains. However, collecting target domain speech-text paired data and retraining the model is often costly and computationally expensive. In this paper, we introduce a simple yet effective method, speech-only adaptation (SOA), based on speech foundation models (Wav2vec 2.0), which requires only speech input data from the target domain. Specifically, the Wav2vec feature encoder is continually pretrained with the Wav2vec loss on both the source and target domain data for domain adaptation, while the contextual encoder is frozen. Compared to a source-domain finetuned model with the feature encoder being frozen during training, we find that simply replacing the frozen feature encoder with the adapted one provides significant WER improvements to the target domain while preserving the performance of the source domain. The effectiveness of this SOA is examined on various low-resource or domain-mismatched ASR settings including adult-child and clean-noisy speech.

This work was presented at the Self-supervision in Audio, Spe