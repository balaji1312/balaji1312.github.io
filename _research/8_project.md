---
layout: page
title: Improving ASR for Child Speech
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 2
category: lab
---

This project presents a novel framework for unsupervised domain adaptation of speech foundation models to low resource domains. Speech foundation models finetuned on certain domains, such as LibriSpeech (adult read speech), behave poorly on other domains (child or noisy speech). One solution could be collecting as much labelled data as possible for joint finetuning on various domains. However, collecting target domain speech-text paired data and retraining the model is often costly and computationally expensive. In this paper, we introduce a simple yet effective method, speech-only adaptation (SOA), based on speech foundation models (Wav2vec 2.0), which requires only speech input data from the target domain. Specifically, the Wav2vec feature encoder is continually pretrained with the Wav2vec loss on both the source and target domain data for domain adaptation, while the contextual encoder is frozen. Compared to a source-domain finetuned model with the feature encoder being frozen during training, we find that simply replacing the frozen feature encoder with the adapted one provides significant WER improvements to the target domain while preserving the performance of the source domain. The effectiveness of this SOA is examined on various low-resource or domain-mismatched ASR settings including adult-child and clean-noisy speech.


This work was presented at the Self-supervision in Audio, Speech and Beyond workshop in ICASSP 2024, and can be accessed <a href="https://arxiv.org/abs/2406.10512"> here</a>


Speech foundation models (SFMs) have achieved state-of-the-art results for various speech tasks in supervised (e.g. Whisper) or self-supervised systems (e.g. WavLM). However, the performance of SFMs for child ASR has not been systematically studied. In addition, there is no benchmark for child ASR with standard evaluations, making the comparisons of novel ideas difficult. In this paper, we initiate and present a comprehensive benchmark on several child speech databases based on various SFMs (Whisper, Wav2vec2.0, HuBERT, and WavLM). Moreover, we investigate finetuning strategies by comparing various data augmentation and parameter-efficient finetuning (PEFT) methods. We observe that the behaviors of these methods are different when the model size increases. For example, PEFT matches the performance of full finetuning for large models but worse for small models. To stabilize finetuning using augmented data, we propose a perturbation invariant finetuning (PIF) loss as a regularization.


Our code can be accessed <a href="https://github.com/balaji1312/SPAPL_KidsASR"> here</a>


This work was presented at Interspeech 2024, and can be accessed <a href="https://arxiv.org/abs/2406.10507"> here</a>