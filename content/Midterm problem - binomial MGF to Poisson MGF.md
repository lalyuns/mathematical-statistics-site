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
  - Poisson limit theorem by MGF
---

# Midterm problem - binomial MGF to Poisson MGF

## Restatement

Find the [[Moment generating function|MGF]] of $X\sim \operatorname{Binomial}(n,p)$, and show that if $n\to\infty$, $p\to 0$, and $np\to\lambda$, then the MGF converges to the Poisson MGF.

## Solution

For a binomial random variable,

$$
M_X(t)=E(e^{tX})=(1-p+pe^t)^n.
$$

Write $p_n$ for the success probability and suppose $np_n\to\lambda$. Then

$$
M_{X_n}(t)
=\left(1+p_n(e^t-1)\right)^n.
$$

Since $p_n(e^t-1)\sim \lambda(e^t-1)/n$,

$$
\left(1+p_n(e^t-1)\right)^n
\to \exp\{\lambda(e^t-1)\}.
$$

This is the MGF of $\operatorname{Poisson}(\lambda)$. Therefore the binomial distribution converges to the Poisson distribution.

## Linked knowledge

- [[Moment generating function]]
- [[Convergence in distribution]]
- [[Common distributions]]

