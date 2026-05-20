---
created: 2026-05-21
categories:
  - Problems
topics:
  - Expectation
tags:
  - statistics
  - midterm
  - conditional-expectation
source:
  - "[[Topic 2 revised]]"
pages:
  - test1_page_020.png
aliases:
  - Mean and variance of a random sum
---

# Midterm problem - random sum mean and variance

## Restatement

Let

$$
T=\sum_{i=1}^N X_i,
$$

where conditional on $N$, the $X_i$ are iid with mean $\mu$ and variance $\sigma^2$. Find $E(T)$ and $\operatorname{Var}(T)$.

## Solution

Condition on $N$:

$$
E(T\mid N)=N\mu.
$$

Using the tower property,

$$
E(T)=E(E(T\mid N))=\mu E(N).
$$

Also,

$$
\operatorname{Var}(T\mid N)=N\sigma^2.
$$

By [[Law of total variance]],

$$
\begin{aligned}
\operatorname{Var}(T)
&=E(\operatorname{Var}(T\mid N))+\operatorname{Var}(E(T\mid N))\\
&=E(N\sigma^2)+\operatorname{Var}(N\mu)\\
&=\sigma^2E(N)+\mu^2\operatorname{Var}(N).
\end{aligned}
$$

## Linked knowledge

- [[Conditional expectation]]
- [[Law of total variance]]
- [[Expectation]]

