---
title: "Maximum Likelihood Estimation & Estimator Distributions in Linear Regression"
excerpt: "Rigorous analysis of OLS and WLS estimators as random variables under homoscedastic and heteroscedastic Gaussian noise conditions.<br/><a href='/files/CIE457_MLE_Project.pdf'>Read the report (PDF)</a>"
collection: portfolio
permalink: /projects/mle-linear-regression/
---

## Overview
[cite_start]This project explores the fundamental principles of Maximum Likelihood Estimation (MLE) in linear regression, focusing on the behavior of estimators as random variables under varying statistical assumptions[cite: 640]. [cite_start]Through mathematical derivation and Monte Carlo simulations ($M = 2000$), we analyze the variance inflation effects of feature correlation and demonstrate the optimal efficiency of Weighted Least Squares (WLS) under heteroscedastic conditions[cite: 177, 641, 644, 648]. [cite_start]Theoretical bounds are verified using the Cramér–Rao Lower Bound (CRLB) and Sufficient Statistics, and real-world complexities are investigated using the classic Engel dataset[cite: 525, 641].

## Highlights
- [cite_start]**MLE & Model Formulation:** Derivation of Ordinary Least Squares (OLS) as the MLE for homoscedastic Gaussian noise [cite: 77][cite_start], and WLS as the MLE for heteroscedastic Gaussian noise[cite: 96].
- [cite_start]**Estimator Distribution Analysis:** Empirical validation proving that OLS and WLS are unbiased estimators whose repeated sampling distributions closely match theoretical Gaussian predictions[cite: 147, 149, 162, 186, 192].
- [cite_start]**Multicollinearity Impact:** Demonstration of how feature correlation inflates individual parameter variances by a factor of $\approx 2.6\times$ while maintaining unbiasedness[cite: 197, 198].
- [cite_start]**Statistical Inference Bounds:** Investigation of 95% Confidence Intervals vs. Prediction Intervals[cite: 361, 415]. [cite_start]Shows how CIs collapse toward zero as $N \to \infty$ while PIs remain constrained by an irreducible noise floor[cite: 649].
- [cite_start]**Real-Data Application:** Diagnostics (Breusch–Pagan test) on the Engel dataset indicating severe heteroscedasticity ($p \approx 0.000$)[cite: 527, 552, 554, 555]. [cite_start]Highlights a critical lesson: data-driven weight estimation introduces its own noise floor, which can inflate empirical standard errors relative to OLS[cite: 581, 583, 584].
- [cite_start]**Advanced Optimality Proofs:** Mathematical verification that both estimators hit the absolute theoretical minimum variance bound ($\text{Cov}(\hat{\beta}) = \mathcal{I}(\beta)^{-1}$) [cite: 689, 700, 704] [cite_start]and compress $N$-dimensional data into $p+1$ scalar sufficient statistics without any loss of information[cite: 739].

## Code
- The code is available on <a href="[https://github.com/taha-at/mle-linear-regression-analysis](https://github.com/taha-at/MLE-Estimation-and-Estimator-Distribution-in-Linear-Regression)">GitHub</a>

## Report
<iframe src="/files/CIE457_MLE_Project.pdf" width="100%" height="900px" style="border:none;"> </iframe>
