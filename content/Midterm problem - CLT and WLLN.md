---
created: 2026-05-21
categories:
  - Problems
topics:
  - Convergence
tags:
  - statistics
  - midterm
  - asymptotics
source:
  - "[[Topic 3 revised]]"
pages:
  - Test2_3_page_001.png
aliases:
  - Law of large numbers and central limit theorem problem
---

# Midterm problem - CLT and WLLN

## Restatement

State the weak law of large numbers and the central limit theorem for iid random variables with finite mean and variance. Use them to justify consistency and asymptotic normality of the sample mean.

## Solution

Let $X_1,X_2,\ldots$ be iid with $E(X_i)=\mu$ and $\operatorname{Var}(X_i)=\sigma^2<\infty$.

The [[Weak law of large numbers]] says

$$
\bar X_n \xrightarrow{p} \mu.
$$

This is consistency of the sample mean.

The [[Central limit theorem]] says

$$
\frac{\sqrt n(\bar X_n-\mu)}{\sigma}\xrightarrow{d}N(0,1).
$$

Equivalently,

$$
\sqrt n(\bar X_n-\mu)\xrightarrow{d}N(0,\sigma^2).
$$

The first result controls the long-run location of $\bar X_n$; the second result describes its first-order fluctuation around $\mu$.

## Linked knowledge

- [[Weak law of large numbers]]
- [[Central limit theorem]]
- [[Convergence in probability]]
- [[Convergence in distribution]]
- [[Quiz problem - convergence in distribution and CLT]]

