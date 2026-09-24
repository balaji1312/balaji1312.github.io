---
layout: page
title: Hallucination Mitigation in Speech Foundation Models
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 3
category: lab
---

Attention encoder-decoder speech foundation models such as Whisper are prone to hallucination: they can emit fluent, confident text on non-speech audio such as noise and music, and they drift from the acoustics on hard inputs like child speech, disfluent speech, and data with imperfect transcripts. This work introduces AURA (Activation-editing with Uncertainty-Routed Adaptation), an ultra-efficient representation-editing method that keeps the pretrained Whisper model frozen and learns sparse scale-and-shift edits for individual decoder cross-attention heads. Static Hard-Concrete gates select which heads are edited, and a token-level dynamic gate decides how strongly each edit applies based on three cross-attention uncertainty signals: over-concentration of attention, diffuse attention, and abrupt shifts in the attended frame. On non-speech audio, AURA sharply reduces the hallucination rate of Whisper-large-v3 without identifying hallucination heads beforehand. On three speech grounding stressors (child speech with imperfect labels on MyST, adult speech with imperfect labels on TED-LIUM 3, and disfluent speech on FluencyBank), it approaches LoRA WER with a small fraction of LoRA's trainable parameters.


This work will be presented at IEEE SLT 2026.


The code can be accessed <a href="https://github.com/balaji1312/aura"> here</a>, and the trained AURA models are available on <a href="https://huggingface.co/balaji1312"> Hugging Face</a>
