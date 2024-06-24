---
layout: page
title: Encoder Only Non-autoregressive ASR 
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 1
category: lab
---

Non-autoregressive automatic speech recognition (NASR) models have gained attention due to their parallelism and fast inference. The encoder-based NASR, e.g. connectionist temporal classification (CTC), can be perfectly initialized from the speech foundation models but does not account for any dependencies among output tokens. The encoder-decoder-based NASR, like CTC alignment-based single-step non-autoregressive transformer (CASS-NAT), can mitigate the dependence problem, but is not able to efficiently integrate speech foundation models. Inspired by the success of recent work of speech-text joint pre-training with a shared transformer encoder, we propose a new encoder-based NASR, UniEnc-CASSNAT, to combine the advantages of CTC and CASS-NAT. UniEnc-CASSNAT consists of only an encoder as the major module, which can be the speech foundation model. The encoder plays the role of both the CASS-NAT encoder and decoder by two forward passes. The first pass of the encoder accepts the speech signal as input, while the concatenation of the speech signal and the token-level acoustic embedding is used as the input for the second pass. Examined on the Librispeech 100h, MyST, and Aishell1 datasets, the proposed UniEnc-CASSNAT achieves state-of-the-art NASR results and is better or comparable to CASS-NAT with only an encoder (fewer model parameters). Our codes can be accessed <a href="https://github.com/balaji1312/cassnat_asr"> here</a>


This work was published in IEEE Signal Processing Letters, and can be accessed <a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10432927">here</a>