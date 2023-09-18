---
layout: page
title: EEG data classification
description: Project for ECE 247 Winter 2022
img: 
importance: 5
category: course
---

In this work, we analyze the classificaiton of EEG data from the BCI Competition using various deep learning architectures. In specific, due to the underlying nature of the dataset, we considered simple sequential architectures such as the Long Short Term Memory (LSTM) and Gated Recurrent Unit (GRU) structures, and investigate equipping these networks with Convolutional layers in the beginning to analyze their performance. In order to capture the spatial pattern present in the data, we explored a transform matrix that is applied to the dataset that converts the 1D EEG data to 2D mesh before feeding into the network models. In addition to comparing different network models, we also considered different pre-processing/data-augmentation techniques such as windowing, GANs/VAEs. We finally show that, data windowing and transformation and followed by CNN with
GRU layers gave us an all subject accuracy of 76.9 %. The trained model and scripts are available <a href="https://github.com/balaji1312/NNDL-proj"> on github </a>
