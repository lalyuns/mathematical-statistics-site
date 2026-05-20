---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
tags:
  - statistics
  - quizzes
  - hypothesis-tests
source:
  - "[[Quiz 2 hypothesis testing problems MOC]]"
pages:
  - "Test3_page_001.png"
---

# Quiz problem - normal interval unbiased test

## Restatement

Let $X_1,\ldots,X_n$ be a random sample from $N(\theta,\sigma^2)$, with known $\sigma^2$. Find an unbiased size $\alpha$ test for

$$
H_0:\theta_1\le\theta\le\theta_2
\qquad\text{versus}\qquad
H_A:\theta<\theta_1\text{ or }\theta>\theta_2.
$$

## Solution

Let $s=\sigma/\sqrt n$ and $\bar X$ be the sample mean. Use a two-tail rejection region

$$
\bar X<c_1
\qquad\text{or}\qquad
\bar X>c_2,
$$

with $c_1<\theta_1<\theta_2<c_2$.

The power function is

$$
\beta(\theta)
=
\Phi\left(\frac{c_1-\theta}{s}\right)
+1-\Phi\left(\frac{c_2-\theta}{s}\right).
$$

Choose $c_1$ and $c_2$ so the boundary null points both have rejection probability $\alpha$:

$$
\beta(\theta_1)=\alpha,
\qquad
\beta(\theta_2)=\alpha.
$$

A symmetric way to write this is to let

$$
m=\frac{\theta_1+\theta_2}{2},\qquad d=\frac{\theta_2-\theta_1}{2s},
$$

and choose $a>d$ such that

$$
\Phi(d-a)+\Phi(-a-d)=\alpha.
$$

Then set

$$
c_1=m-as,\qquad c_2=m+as.
$$

This gives a size $\alpha$ test. It is unbiased because outside the interval the rejection probability is at least the boundary value $\alpha$, while inside the interval the maximum rejection probability is attained at the boundary.

## Links

- [[Unbiased test]]
- [[Size and level]]
- [[Rejection region]]
- [[Power function]]
