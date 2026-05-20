---
created: 2026-05-21
categories:
  - Problems
topics:
  - Probability
tags:
  - statistics
  - midterm
  - distributions
source:
  - "[[Topic 1 revised]]"
pages:
  - Test2_1_page_001.png
aliases:
  - Cauchy distribution from arctangent CDF
---

# Midterm problem - Cauchy CDF and density

## Restatement

Show that

$$
F(x)=\frac{1}{2}+\frac{1}{\pi}\tan^{-1}(x),\qquad -\infty<x<\infty,
$$

is a valid [[CDF]], then find the corresponding [[PDF and PMF|density]].

## Solution

The limits are

$$
\lim_{x\to -\infty}F(x)=0,\qquad \lim_{x\to\infty}F(x)=1,
$$

because $\tan^{-1}(x)\to -\pi/2$ and $\tan^{-1}(x)\to \pi/2$.

Also,

$$
F'(x)=\frac{1}{\pi(1+x^2)}>0,
$$

so $F$ is increasing. Since $F$ is continuous, it is right-continuous. Therefore $F$ is a valid CDF.

The density is

$$
f(x)=F'(x)=\frac{1}{\pi(1+x^2)},\qquad -\infty<x<\infty.
$$

This is the standard Cauchy density.

## Linked knowledge

- [[CDF]]
- [[PDF and PMF]]
- [[Common distributions]]

