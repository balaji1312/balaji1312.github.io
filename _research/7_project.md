---
layout: page
title: Dialect Density Estimation for African American English
description: Work with Speech Processing and Auditory Perception Lab at UCLA
img: 
importance: 5
category: lab
---

This project evaluates a novel framework for spoken dialect density prediction on both children's and adult's African American English.  A speaker's dialect density is defined as the frequency with which dialect-specific language characteristics occur in their speech.  Rather than treating the presence or absence of a target dialect in a user's speech as a binary decision, we instead train a classifier to predict the level of dialect density in order to provide a higher degree of specificity in down-stream tasks.  For this, we experiment with self-supervised learning representations from HuBERT, hand-crafted grammar-based features extracted from ASR transcripts, prosodic features, and other feature sets as the input to an XGBoost classifier. We then train the classifier to assign dialect density labels to 1-2 minute recorded utterances. We achieve high dialect density level classification accuracy for both child and adult speech and demonstrate robust performance across age and regional variations of dialect.


This work was published in The Journal of the Acoustical Society of America, and can be accessed <a href="https://pubs.aip.org/asa/jasa/article/155/4/2836/3286597/An-exploratory-study-on-dialect-density-estimation"> here</a>