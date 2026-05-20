---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - estimation
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_003.png
aliases:
  - UMVUE orthogonality characterization
---

# UMVUE characterization

An unbiased estimator $W$ is the [[UMVUE]] of $\tau(\theta)$ iff it is uncorrelated with every unbiased estimator of zero.

That is, for every statistic $U$ such that $E_\theta[U]=0$ for all $\theta$,

$$
\operatorname{Cov}_\theta(W,U)=0.
$$

## Why this proves minimum variance

If $W^*$ is another unbiased estimator of $\tau(\theta)$, then

$$
U=W^*-W
$$

is an unbiased estimator of zero. Orthogonality gives

$$
\operatorname{Var}_\theta(W^*)
=\operatorname{Var}_\theta(W+U)
=\operatorname{Var}_\theta(W)+\operatorname{Var}_\theta(U)
\ge \operatorname{Var}_\theta(W).
$$

Conversely, if $W$ is UMVUE and $U$ is unbiased for zero, then $W+aU$ is unbiased for $\tau(\theta)$ for every real $a$. The variance

$$
\operatorname{Var}_\theta(W+aU)
=\operatorname{Var}_\theta(W)+2a\operatorname{Cov}_\theta(W,U)+a^2\operatorname{Var}_\theta(U)
$$

must be minimized at $a=0$, so the linear coefficient must be zero. Hence $\operatorname{Cov}_\theta(W,U)=0$.

Related: [[UMVUE]], [[Lehmann-Scheffe theorem]], [[Unbiased estimator of zero]].
