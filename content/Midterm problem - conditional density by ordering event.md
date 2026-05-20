---
created: 2026-05-21
categories:
  - Problems
topics:
  - Joint distributions
tags:
  - statistics
  - midterm
  - conditional-distributions
source:
  - "[[Topic 2 revised]]"
pages:
  - Test2_2_page_001.png
aliases:
  - Density of X conditioned on X greater than Y
---

# Midterm problem - conditional density by ordering event

## Restatement

Let $X$ and $Y$ be independent continuous random variables with densities $f$ and $g$, and CDFs $F$ and $G$. Find the density of $X$ conditional on $X>Y$, and the density of $X$ conditional on $X\leq Y$.

## Solution

For a small interval around $x$,

$$
P(x<X<x+dx,\ X>Y)\approx f(x)P(Y<x)\,dx=f(x)G(x)\,dx.
$$

Thus

$$
f_{X\mid X>Y}(x)
=\frac{f(x)G(x)}{P(X>Y)}
=\frac{f(x)G(x)}{\int_{-\infty}^{\infty} f(t)G(t)\,dt}.
$$

Similarly,

$$
P(x<X<x+dx,\ X\leq Y)\approx f(x)P(Y\geq x)\,dx=f(x)(1-G(x))\,dx.
$$

Therefore

$$
f_{X\mid X\leq Y}(x)
=\frac{f(x)(1-G(x))}
{\int_{-\infty}^{\infty} f(t)(1-G(t))\,dt}.
$$

## Linked knowledge

- [[Joint distribution]]
- [[Conditional distribution]]
- [[Independence]]

