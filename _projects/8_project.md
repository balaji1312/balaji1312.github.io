---
layout: page
title: Hedging in fractional Black–Scholes model with transaction costs
description: Project for ECE 239AS Fall 2022
img: 
importance: 4
category: course
---

Through this project, we aim to analyze and implement the paper _Hedging in fractional Black–Scholes model with transaction costs_ by critically analyzing the proofs, and corollaries listed in the paper. Concepts such as Brownian motion and martingale provided a solid foundation for understanding the paper’s analysis of the fractional Black-Scholes model through modelling the underlying stochastic dynamics of the fluctuations in call options. 

The presence of transaction costs implies that a conditional mean hedging strategy is required for an optimal trading for a given fixed strike price of the underlying stock. 
We alse tested the validity of the claims made in the paper by simulating a toy model for European call options. We evaluate the stochastic integrals present in the optimal strategy by solving the Ito equation for fBM by using the Euler-Maruyama algorithm. We observe that as expected the value of the fluctuations of the fBM, and the tracking ability of the martingale adapted to the given filtration, are tied to the Hurst index H 