---
created: 2026-05-21
categories:
  - Problems
topics:
  - Probability
tags:
  - statistics
  - midterm
  - mgfs
source:
  - "[[Topic 2 revised]]"
pages:
  - Test2_1_page_001.png
aliases:
  - Poisson sums by MGF
---

# Midterm problem - sum of independent Poissons

## Restatement

Let $X_1,\ldots,X_n$ be independent with $X_i\sim \operatorname{Poisson}(\lambda_i)$. Find the distribution of

$$
Y=\sum_{i=1}^n X_i.
$$

## Solution

The Poisson MGF is

$$
M_{X_i}(t)=\exp\{\lambda_i(e^t-1)\}.
$$

By [[Independence]], the MGF of a sum is the product of the MGFs:

$$
\begin{aligned}
M_Y(t)
&=\prod_{i=1}^n M_{X_i}(t)\\
&=\prod_{i=1}^n \exp\{\lambda_i(e^t-1)\}\\
&=\exp\left\{\left(\sum_{i=1}^n\lambda_i\right)(e^t-1)\right\}.
\end{aligned}
$$

This is the MGF of

$$
Y\sim \operatorname{Poisson}\left(\sum_{i=1}^n\lambda_i\right).
$$

## Linked knowledge

- [[Moment generating function]]
- [[Independence]]
- [[Common distributions]]

