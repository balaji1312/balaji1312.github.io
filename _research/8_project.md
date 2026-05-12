---
layout: page
title: Improving ASR for Child Speech
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 6
category: lab
---

Speech foundation models finetuned on certain domains, such as LibriSpeech (adult read speech), behave poorly on other domains (child or noisy speech). One solution could be collecting as much labelled data as possible for joint finetuning on various domains. However, collecting target domain speech-text paired data and retraining the model is often costly and computationally expensive. In this paper, we introduce a simple yet effective method, speech-only adaptation (SOA), based on speech foundation models (Wav2vec 2.0), which requires only speech input data from the target domain. Specifically, the Wav2vec feature encoder is continually pretrained with the Wav2vec loss on both the source and target domain data for domain adaptation, while the contextual encoder is frozen. Compared to a source-domain finetuned model with the feature encoder being frozen during training, we find that simply replacing the frozen feature encoder with the adapted one provides significant WER improvements to the target domain while preserving the performance of the source domain. The effectiveness of this SOA is examined on various low-resource or domain-mismatched ASR settings including adult-child and clean-noisy speech.


This work was presented at the Self-supervision in Audio, Speech and Beyond workshop in ICASSP 2024, and can be accessed <a href="https://ieeexplore.ieee.org/document/10625884"> here</a>


Speech foundation models (SFMs) have achieved state-of-the-art results for various speech tasks in supervised (e.g. Whisper) or self-supervised systems (e.g. WavLM). However, the performance of SFMs for child ASR has not been systematically studied. In addition, there is no benchmark for child ASR with standard evaluations, making the comparisons of novel ideas difficult. In this paper, we initiate and present a comprehensive benchmark on several child speech databases based on various SFMs (Whisper, Wav2vec2.0, HuBERT, and WavLM). Moreover, we investigate finetuning strategies by comparing various data augmentation and parameter-efficient finetuning (PEFT) methods. We observe that the behaviors of these methods are different when the model size increases. For example, PEFT matches the performance of full finetuning for large models but worse for small models. To stabilize finetuning using augmented data, we propose a perturbation invariant finetuning (PIF) loss as a regularization.


Our code can be accessed <a href="https://github.com/balaji1312/SPAPL_KidsASR"> here</a>


This work was presented at Interspeech 2024, and can be accessed <a href="https://www.isca-archive.org/interspeech_2024/fan24b_interspeech.html"> here</a>


A follow-up study examines how self-supervised speech representations shift across speaker age and how that shift drives ASR degradation on child speech. We introduce Delta SSL embeddings, frame-level differences between SSL representations of an utterance and a reference, and show that incorporating these delta features into ASR training improves robustness on children's speech without retraining the underlying foundation model — a practical recipe when target-domain labeled data is scarce.


This work was presented at ICASSP 2026, and can be accessed <a href="https://ieeexplore.ieee.org/document/11462835"> here</a>


A collaborative effort with the ESPnet community provides a systematic benchmark of training paradigms, dataset compositions, and model scaling for child ASR within the ESPnet toolkit. The study covers supervised vs. self-supervised pretraining, multi-corpus mixing strategies, and parameter scaling across model sizes, providing reproducible recipes and baselines that the broader community can build on for child ASR research.


This work was presented at WOCCI 2025, and can be accessed <a href="https://www.isca-archive.org/wocci_2025/ying25_wocci.html"> here</a>
