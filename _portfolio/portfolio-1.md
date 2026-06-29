---
title: "Maximum Likelihood Estimation & Estimator Distributions in Linear Regression"
excerpt: "Rigorous analysis of OLS and WLS estimators as random variables under homoscedastic and heteroscedastic Gaussian noise conditions.<br/><a href='/files/CIE457_MLE_Project.pdf'>Read the report (PDF)</a>"
collection: portfolio
permalink: /projects/mle-linear-regression/
---

## Overview
This project explores the fundamental principles of Maximum Likelihood Estimation (MLE) in linear regression, focusing on the behavior of estimators as random variables under varying statistical assumptions. Through mathematical derivation and Monte Carlo simulations ($M = 2000$), we analyze the variance inflation effects of feature correlation and demonstrate the optimal efficiency of Weighted Least Squares (WLS) under heteroscedastic conditions. Theoretical bounds are verified using the Cramér–Rao Lower Bound (CRLB) and Sufficient Statistics, and real-world complexities are investigated using the classic Engel dataset.

## Highlights
- **MLE & Model Formulation:** Derivation of Ordinary Least Squares (OLS) as the MLE for homoscedastic Gaussian noise, and WLS as the MLE for heteroscedastic Gaussian noise.
- **Estimator Distribution Analysis:** Empirical validation proving that OLS and WLS are unbiased estimators whose repeated sampling distributions closely match theoretical Gaussian predictions.
- **Multicollinearity Impact:** Demonstration of how feature correlation inflates individual parameter variances by a factor of $\approx 2.6\times$ while maintaining unbiasedness.
- **Statistical Inference Bounds:** Investigation of 95% Confidence Intervals vs. Prediction Intervals. Shows how CIs collapse toward zero as $N \to \infty$ while PIs remain constrained by an irreducible noise floor.
- **Real-Data Application:** Diagnostics (Breusch–Pagan test) on the Engel dataset indicating severe heteroscedasticity ($p \approx 0.000$). Highlights a critical lesson: data-driven weight estimation introduces its own noise floor, which can inflate empirical standard errors relative to OLS.
- **Advanced Optimality Proofs:** Mathematical verification that both estimators hit the absolute theoretical minimum variance bound ($\text{Cov}(\hat{\beta}) = \mathcal{I}(\beta)^{-1}$) and compress $N$-dimensional data into $p+1$ scalar sufficient statistics without any loss of information.

## Code
- The code is available on <a href="https://github.com/taha-at/mle-linear-regression-analysis">GitHub</a>

## Report
<iframe src="/files/CIE457_MLE_Project.pdf" width="100%" height="900px" style="border:none;"> </iframe>
