---
layout: page
title: Neural Speech and Audio Coding
description: Work with the Speech Processing and Auditory Perception Lab at UCLA and Qualcomm
img: 
importance: 3
category: lab
---

Neural audio codecs compress audio into discrete tokens that can be fed directly into token-based language models, but they face a fundamental tradeoff: traditional codecs preserve acoustic detail well yet carry little semantic information, while recent hybrid codecs add semantics through distillation at the cost of reconstruction quality. This work introduces STACodec, a unified codec that injects semantic information from self-supervised learning models into the first layer of residual vector quantization through semantic token assignment. To remove the reliance on an external SSL tokenizer and stay efficient at inference, a semantic pre-distillation module predicts the semantic tokens directly for assignment to the first quantization layer. STACodec outperforms existing hybrid codecs on both audio reconstruction and downstream semantic tasks, striking a better balance between acoustic fidelity and semantic capability.


This work was presented at ICASSP 2026, and can be accessed <a href="https://arxiv.org/abs/2602.06180"> here</a>


The code can be accessed <a href="https://github.com/epcm/STACodec"> here</a>


A related strand of this work comes from a summer 2025 research internship at Qualcomm's Audio & ML Research group in San Diego, focused on neural speech coding. The internship developed and optimized multi-bitrate speech coding methods aimed at practical deployment in resource-constrained conditions, exploring novel approaches to balance speech quality against bitrate efficiency in low-resource scenarios. Codec performance was designed and evaluated under challenging real-world conditions, including background noise, packet loss, and speaker variability.
