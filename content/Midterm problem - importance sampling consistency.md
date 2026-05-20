---
created: 2026-05-21
categories:
  - Problems
topics:
  - Convergence
tags:
  - statistics
  - midterm
  - monte-carlo
source:
  - "[[Topic 3 revised]]"
pages:
  - test1_page_022.png
aliases:
  - Importance sampling estimator converges in probability
---

# Midterm problem - importance sampling consistency

## Restatement

Let

$$
I(f)=\int_a^b f(x)\,dx.
$$

Suppose $X_1,\ldots,X_n$ are iid from a density $g$ that is positive wherever $f$ is nonzero. Show that

$$
\hat I_n=\frac{1}{n}\sum_{i=1}^n \frac{f(X_i)}{g(X_i)}
$$

converges in probability to $I(f)$.

## Solution

Define

$$
W_i=\frac{f(X_i)}{g(X_i)}.
$$

Under sampling from $g$,

$$
E_g(W_i)=\int \frac{f(x)}{g(x)}g(x)\,dx=\int_a^b f(x)\,dx=I(f).
$$

The estimator is the sample mean of the $W_i$:

$$
\hat I_n=\bar W_n.
$$

By the [[Weak law of large numbers]],

$$
\hat I_n=\bar W_n\xrightarrow{p}E(W_i)=I(f),
$$

provided the required finite mean condition holds.

## Linked knowledge

- [[Expectation]]
- [[Weak law of large numbers]]
- [[Convergence in probability]]

