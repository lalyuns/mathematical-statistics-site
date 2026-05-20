---
created: 2026-05-21
categories:
  - Problems
topics:
  - Probability
tags:
  - statistics
  - midterm
  - transformations
source:
  - "[[Topic 1 revised]]"
pages:
  - Test2_1_page_001.png
aliases:
  - CDF transform gives a uniform random variable
---

# Midterm problem - probability integral transform

## Restatement

Let $X$ be continuous with strictly increasing CDF $F$. Find the distribution of

$$
U=F(X).
$$

## Solution

For $0<u<1$,

$$
\begin{aligned}
P(U\leq u)
&=P(F(X)\leq u)\\
&=P(X\leq F^{-1}(u))\\
&=F(F^{-1}(u))\\
&=u.
\end{aligned}
$$

Thus $U\sim \operatorname{Uniform}(0,1)$.

The inverse version is [[Inverse transform sampling]]: if $U\sim \operatorname{Uniform}(0,1)$, then $F^{-1}(U)$ has CDF $F$.

## Linked knowledge

- [[Probability integral transform]]
- [[Inverse transform sampling]]
- [[CDF]]

