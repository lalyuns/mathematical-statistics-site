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
  - Topic 4_revised_page_002.png
  - Topic 4_revised_page_003.png
---

# Cramer-Rao lower bound

For an unbiased estimator $W$ of $\tau(\theta)$,

$$
\operatorname{Var}_\theta(W)\ge \frac{[\tau'(\theta)]^2}{I(\theta)}.
$$

The bound is governed by Fisher information $I(\theta)$.

For iid data, Topic 4 writes the one-observation information as $I_0(\theta)$, so the bound is

$$
\operatorname{Var}_\theta(W)\ge \frac{[\tau'(\theta)]^2}{nI_0(\theta)}.
$$

## Proof skeleton with missing steps

Let

$$
S_n(\theta)=\partial_\theta\sum_{i=1}^n\log f(X_i\mid\theta)
$$

be the sample [[Score function]]. Since $W$ is unbiased,

$$
E_\theta[W]=\tau(\theta).
$$

Differentiate both sides. Under [[Regularity conditions]], the derivative passes inside the integral:

$$
\tau'(\theta)
=\partial_\theta E_\theta[W]
=E_\theta[W S_n(\theta)].
$$

Also $E_\theta[S_n(\theta)]=0$, so

$$
E_\theta[W S_n(\theta)]
=\operatorname{Cov}_\theta(W,S_n(\theta)).
$$

By Cauchy-Schwarz,

$$
[\tau'(\theta)]^2
\le \operatorname{Var}_\theta(W)\operatorname{Var}_\theta(S_n(\theta)).
$$

For iid samples,

$$
\operatorname{Var}_\theta(S_n(\theta))=nI_0(\theta).
$$

Rearranging gives the lower bound. The equality case is [[CRLB equality condition]].

Related: [[UMVUE]], [[Fisher information]], [[Score function]], [[Regularity conditions]], [[Asymptotic normality of MLE]].
