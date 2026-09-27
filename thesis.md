# New Heavy-Tailed Distribution Families

**MSc Thesis — Statistics, BIUST**
Supervisors: Dr F. Chipepa, Prof B. Oluyede · Submitted March 2025

## The Problem

Standard distributions used across reliability engineering, medicine, and finance — Weibull, Pareto, log-logistic — each break down in a specific way once real data gets extreme. Weibull's tail decays too fast to capture rare, severe outliers. Pareto's shape is too rigid to adapt across different datasets. Log-logistic handles skew but under-represents true tail risk.

## What I Built

I derived and fully characterized three new distribution families:

- **HT-TIITL-G** (Heavy-Tailed-Type II Topp-Leone-G) — combines the heavy-tailed transformation with the Type II Topp-Leone family, adding two shape parameters that let the same family fit increasing, decreasing, and bathtub-shaped hazard rates.
- **HT-TIITL-GPS** (Power Series extension) — extended with a power-series component for datasets with an unknown number of underlying risk factors.
- **TL-GEHL-G** (Topp-Leone-Generalized Exponentiated Half Logistic-G) — built on the half-logistic distribution, for positively-skewed data like income, insurance claims, and response times.

For each family, I derived the quantile function, moment generating function, linear representation, order statistics, and Rényi entropy — then estimated parameters with maximum likelihood estimation (MLE) and validated the estimator with Monte Carlo simulation across seven sample sizes (n = 25 to 1000, 3,000 replications each).

## Results on Real Data

I tested the lead family (HT-TIITL-W) against four established models (Weibull, HLGW, TI-HTW, HT-BPTW) on two real datasets:

**Reliability engineering** (machine failure times, n=30): HT-TIITL-W had the lowest −2log-likelihood (327.3) and highest K–S p-value (0.8267) of all five models.

**Cancer patient remission times** (n=128 patients): K–S p-value of **0.9997** vs. Weibull's 0.5573 — a near-perfect fit on real clinical data.

## Skills Demonstrated

Statistical modeling · Maximum likelihood estimation · Monte Carlo simulation · Goodness-of-fit testing · Survival analysis · R programming
