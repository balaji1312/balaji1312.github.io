---
layout: page
title: Automatic Separation of Vocal and Non-Vocal Segments Present in South Indian Songs  
description: Work with Pattern Recognition and Computational Intelligence Laboratory at NIT Trichy
img: 
importance: 8
category: lab
---

This goal of this project was to build a backend semgementation system capable of distinguishing voice and non-voiced audio segments in the presence of background instrumental noise. To achieve this, MFCCs were extracted from all segments for isolation of lower frequencies present by discarding high filter banks. Different classifiers were then experimented with for cleaner feature seaparation. Ultimately, an SVM with a modified Gaussian kernel was chosen and was able to achieve a segment level classification accuracy of 82%, a 17% improvement over a standard Gaussian kernel. 