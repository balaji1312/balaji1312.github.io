---
layout: page
title: Noise Robust Automatic Speech Recognition
description: Project for ECE 214A Spring 2022
img: 
importance: 3
category: course
---

The goal of this course project was to perform ASR on a set of words from the Common Voice database with added babble noise. To do this, our approach focused on augmenting the clean data with Pink Noise and a custom noise reduction pipeline using a combination of Gammatone Coefficients, Quartile Normalization and Rasta Filtering. 

Ultimately we were able to reduce the Word Error Rate by 36% relative to the baseline. The trained model and scripts are available <a href="https://github.com/balaji1312/noisy-asr"> on github </a>
