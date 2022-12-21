---
layout: page
title: Data Compression using Online Linear Classifier
description: Project for ECE 236 Fall 2021
img: 
importance: 3
category: course
---

The goal of this course project was to create a classifier for the MNIST database that attempted to answer two questions: 1) Given a predetermined classifier, will the addition of a new point to the training set meaningfully improve its accuracy?, and 2) Given a particular training set, what is the minimum number of points necessary from the given set necesary to achieve a threshold accuracy? We attempt to answer both these questions using Linear Programming concepts by designing a optimisation problem that can be colved using cvxpy.

By essentially computes the Mahalanobis distance to check the optimality of a new point, we were able to developed an online classifier to reduce data transmission and achieve an accuracy of 98.1% on MNIST dataset, while drastically compressing data required by using only 0.23% of all available samples. The implemenetation for both 'parts' of the project are available <a href="https://github.com/balaji1312/compressed-online-classifier"> here </a>