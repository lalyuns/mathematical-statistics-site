---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Expectation]]"
tags:
  - statistics
  - mgf
source:
  - "[[Topic 2 revised]]"
---

# Moment generating function

The moment generating function of $X$ is

$$
M_X(t)=E[e^{tX}]
$$

when it exists near $0$.

It determines the distribution and turns independent sums into products:

$$
M_{X+Y}(t)=M_X(t)M_Y(t).
$$

If $M_X(t)$ exists near $0$, its derivatives at $0$ recover moments:

$$
M_X'(0)=E[X],\qquad M_X''(0)=E[X^2].
$$

For iid sums, this product rule is what makes the MGF proof of [[Central limit theorem]] work.

Related: [[MGF continuity theorem]], [[Central limit theorem]], [[Midterm problem - sum of independent Poissons]], [[Midterm problem - binomial MGF to Poisson MGF]].
