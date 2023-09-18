---
layout: page
title: Gene compression using Machine Learning for Cancer type Classification
description: Project for BIOENG 275 Fall 2022
img: 
importance: 7
category: course
---

In this project, we focus on using compression algorithms to capture latent features in gene data. These features reveal valuable information about the genomic space and can be used to generate hypotheses and develop robust models for cancer type classification. We also focus on using RNAseq data for this task. Overall, our approach allows us to better understand the genomic space and improve cancer type classification.

To achieve this, we trained three compression algorithms - PCA, ICA, NMF - on the TCGA dataset, and evaluated them across different metrics. We found that certain dimensionalities were optimal for each algorithm, and we used these to identify the best biological representations. Our approach achieved 92.22% accuracy for predicting cancer types. Overall, our study showed that the use of compression algorithms can help to improve the accuracy of cancer type prediction. The trained model and scripts are available <a href="https://github.com/balaji1312/gene-compression"> on github </a>
