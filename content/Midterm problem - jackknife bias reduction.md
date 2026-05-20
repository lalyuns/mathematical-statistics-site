---
created: 2026-05-21
categories:
  - Problems
topics:
  - Point estimation
tags:
  - statistics
  - midterm
  - bias
source:
  - "[[Topic 4 revised]]"
pages:
  - test1_page_024.png
aliases:
  - Jackknife removes first-order bias
---

# Midterm problem - jackknife bias reduction

## Restatement

Suppose an estimator $\hat\theta$ based on $n=mp$ observations has bias expansion

$$
E(\hat\theta)-\theta=\frac{b_1(\theta)}{n}+O(n^{-2}).
$$

Split the data into $p$ groups of size $m$. Let $\hat\theta_{(j)}$ be the estimator that leaves out group $j$, so it is based on $n-m=n(p-1)/p$ observations. Define the jackknife estimator using pseudo-values

$$
V_j=p\hat\theta-(p-1)\hat\theta_{(j)},\qquad
\hat\theta_J=\frac{1}{p}\sum_{j=1}^p V_j.
$$

Show that the first-order bias is removed.

## Solution

The full estimator satisfies

$$
E(\hat\theta)=\theta+\frac{b_1(\theta)}{n}+O(n^{-2}).
$$

The leave-one-group estimator uses $n(p-1)/p$ observations, so

$$
E(\hat\theta_{(j)})
=\theta+\frac{b_1(\theta)}{n(p-1)/p}+O(n^{-2})
=\theta+\frac{p\,b_1(\theta)}{n(p-1)}+O(n^{-2}).
$$

Then

$$
\begin{aligned}
E(V_j)
&=pE(\hat\theta)-(p-1)E(\hat\theta_{(j)})\\
&=p\left(\theta+\frac{b_1}{n}+O(n^{-2})\right)
-(p-1)\left(\theta+\frac{p b_1}{n(p-1)}+O(n^{-2})\right)\\
&=\theta+O(n^{-2}).
\end{aligned}
$$

Averaging the pseudo-values preserves this order:

$$
E(\hat\theta_J)=\theta+O(n^{-2}).
$$

Thus the jackknife cancels the $1/n$ bias term.

## Linked knowledge

- [[Bias variance MSE decomposition]]
- [[Point estimation]]
- [[Expectation]]

