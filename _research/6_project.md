---
layout: page
title: Question Answering from Long Audio Files
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 4
category: lab
---

This project presents a novel dataset (CORAAL QA) and framework for audio question-answering from long audio recordings containing spontaneous speech.  The dataset introduced here provides sets of questions that can be factually answered from short spans of a long audio files (typically 30min to 1hr) from the Corpus of Regional African American Language.  Using this dataset, we divide the audio recordings into 60 second segments, automatically transcribe each segment, and use PLDA scoring of BERT-based semantic embeddings to rank the relevance of ASR transcript segments in answering the target question.  In order to improve this framework through data augmentation, we use large language models including ChatGPT and Llama 2 to automatically generate further training examples and show how prompt engineering can be optimized for this process.  By creatively leveraging knowledge from large-language models, we achieve state-of-the-art question-answering performance in this information retrieval task.


Our database can be accessed <a href="https://github.com/balaji1312/CORAAL-QA"> here</a>


This work was presented at ICASSP 2024, and can be accessed <a href="https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10447109"> here</a>