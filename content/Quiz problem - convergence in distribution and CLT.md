---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
tags:
  - statistics
  - quizzes
  - asymptotics
source:
  - "[[Quiz 2 hypothesis testing problems MOC]]"
pages:
  - "Test1_page_001.png"
  - "Test4_page_001.png"
  - "Test5_page_001.png"
---

# Quiz problem - convergence in distribution and CLT

## Restatement

Several Quiz 2 pages ask for asymptotic facts connected to [[Asymptotic test]]:

- Define convergence in distribution.
- Show that if $X_1,\ldots,X_n$ have mean $\mu$ and variance $\sigma^2$, then

$$
\frac{\sqrt n(\bar X_n-\mu)}{\sigma}\xrightarrow{d}N(0,1).
$$

## Solution

Random variables $Y_n$ converge in distribution to $Y$, written

$$
Y_n\xrightarrow{d}Y,
$$

if

$$
F_{Y_n}(y)\to F_Y(y)
$$

at every continuity point $y$ of $F_Y$.

For iid $X_i$ with $E[X_i]=\mu$ and $\operatorname{Var}(X_i)=\sigma^2<\infty$, the central limit theorem gives

$$
\frac{\sum_{i=1}^n X_i-n\mu}{\sigma\sqrt n}
\xrightarrow{d}N(0,1).
$$

Since

$$
\frac{\sum_{i=1}^n X_i-n\mu}{\sigma\sqrt n}
=
\frac{\sqrt n(\bar X_n-\mu)}{\sigma},
$$

the desired result follows.

This is the basic asymptotic logic behind many large-sample tests, including tests justified by [[Wilks theorem]].

## Links

- [[Asymptotic test]]
- [[Wilks theorem]]
- [[Exact test]]
