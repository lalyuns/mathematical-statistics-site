---
created: 2026-05-21
categories:
  - Problems
topics:
  - Probability
tags:
  - statistics
  - midterm
  - poisson-processes
source:
  - "[[Topic 2 revised]]"
pages:
  - Test2_2_page_001.png
aliases:
  - First arrival time in a Poisson process
---

# Midterm problem - Poisson process waiting time

## Restatement

Let $N(t)$ be a Poisson process with rate $\lambda$. Derive the distribution of the first waiting time

$$
T_1=\inf\{t:N(t)\geq 1\}.
$$

## Solution

The event $T_1>t$ means that no event has occurred by time $t$:

$$
P(T_1>t)=P(N(t)=0).
$$

Since $N(t)\sim \operatorname{Poisson}(\lambda t)$,

$$
P(N(t)=0)=e^{-\lambda t}.
$$

Therefore the CDF is

$$
F_{T_1}(t)=1-e^{-\lambda t},\qquad t\geq 0.
$$

Differentiating gives

$$
f_{T_1}(t)=\lambda e^{-\lambda t},\qquad t\geq 0.
$$

So $T_1\sim \operatorname{Exponential}(\lambda)$.

## Linked knowledge

- [[CDF]]
- [[PDF and PMF]]
- [[Common distributions]]

