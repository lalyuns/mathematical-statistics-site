---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Expectation]]"
tags:
  - statistics
  - asymptotics
source:
  - "[[Topic 2 revised]]"
---

# Delta method

[[Delta method]] approximates a transformed statistic using Taylor expansion.

If $\sqrt n(Y_n-\mu)\xrightarrow{d}N(0,\sigma^2)$ and $g'(\mu)\ne0$, then

$$
\sqrt n(g(Y_n)-g(\mu))\xrightarrow{d}N(0,\sigma^2[g'(\mu)]^2).
$$

If $g'(\mu)=0$, second-order expansion is needed.
