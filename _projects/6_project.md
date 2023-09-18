---
layout: page
title: SSL Representations of Speech for Depression Detection and Children ASR
description: Project for ECE 214B Spring 2023
img: 
importance: 2
category: course
---

For this course, we worked on two different projects focused on different representations of speech in speech foundation models: Depression detection, and ASR of child speech

Project 1 consisted of working on depression detection through the analysis of speech signals, employing the Emotional Audio-Textual Depression Dataset (EATD) Corpus. We attempted to employ different techniques to extract various acoustic features from the provided waveforms, and adjustments to the epochs were made to optimize the outcomes. The results of extensive experimentation indicate that the comparE16 technique yielded the highest accuracy, with an impressive F1 average score of 0.6228. 

In Project 2 we work on the recent research on SSL for child ASR and explore its impact on ASR system accuracy. We use the Librispeech and MyST datasets for training and evaluating ASR models on adult and child speech respectively. Data augmentation techniques, including VTLP, SpecAugment, spectral warping, and pitch
perturbation, are employed to enhance the performance of ASR models. The final part of the project includes a layerwise analysis of SSL models using Canonical Correlation Analysis to understand information propagation and feature extraction within the models. 

The trained model and scripts for both projects are available <a href="https://github.com/balaji1312/adv-speech-processing"> on github </a>
