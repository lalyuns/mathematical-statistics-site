---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - likelihood
  - estimation
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_002.png
  - Topic 4_revised_page_007.png
---

# Score function

The [[Score function]] is the derivative of the log-likelihood:

$$
S(\theta)=\partial_\theta \ell(\theta),
\qquad
\ell(\theta)=\sum_{i=1}^n\log f(X_i\mid\theta).
$$

For one observation, the score is

$$
s_\theta(X)=\partial_\theta\log f(X\mid\theta).
$$

Under regularity conditions that allow differentiation under the integral sign,

$$
E_\theta[s_\theta(X)]
=\int \partial_\theta\log f(x\mid\theta)f(x\mid\theta)\,dx
=\int \partial_\theta f(x\mid\theta)\,dx
=\partial_\theta\int f(x\mid\theta)\,dx
=0.
$$

This zero-mean property is the hidden step behind the [[Cramer-Rao lower bound]] proof and the asymptotic normality proof for MLEs.

Related: [[Fisher information]], [[Regularity conditions]], [[Likelihood function]].
