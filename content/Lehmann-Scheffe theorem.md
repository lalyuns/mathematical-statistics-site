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
  - Topic 4_revised_page_005.png
---

# Lehmann-Scheffe theorem

If $S$ is complete and sufficient, and $\phi(S)$ is unbiased for $\tau(\theta)$, then $\phi(S)$ is the [[UMVUE]].

This theorem turns completeness plus sufficiency into uniqueness and minimum variance.

## Proof skeleton with missing steps

Let $U$ be any [[Unbiased estimator of zero]]. To use [[UMVUE characterization]], it is enough to prove

$$
E_\theta[\phi(S)U]=0.
$$

Condition on $S$:

$$
E_\theta[\phi(S)U]
=E_\theta[\phi(S)E_\theta(U\mid S)].
$$

Now $E_\theta(U\mid S)$ is a function of $S$. Also

$$
E_\theta[E_\theta(U\mid S)]=E_\theta(U)=0
$$

for all $\theta$. By [[Completeness]], this forces

$$
E_\theta(U\mid S)=0
$$

almost surely. Therefore $E_\theta[\phi(S)U]=0$, and $\phi(S)$ is the UMVUE.

Related: [[Rao-Blackwell theorem]], [[Factorization theorem]], [[Completeness]], [[UMVUE characterization]], [[Natural exponential family]].
