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
  - Cramer-Rao equality condition
---

# CRLB equality condition

An unbiased estimator $W$ attains the [[Cramer-Rao lower bound]] exactly when the Cauchy-Schwarz inequality used in the proof is an equality.

For iid one-parameter models, equality holds iff

$$
W(X)-\tau(\theta)=a(\theta)\sum_{i=1}^n \partial_\theta\log f(X_i\mid\theta)
$$

for some function $a(\theta)$.

Why: the proof bounds

$$
|\operatorname{Cov}_\theta(W,S_n(\theta))|^2
\le \operatorname{Var}_\theta(W)\operatorname{Var}_\theta(S_n(\theta)),
$$

where $S_n(\theta)$ is the sample score. Cauchy-Schwarz is equality exactly when $W-\tau(\theta)$ is proportional to $S_n(\theta)$ almost surely.

Related: [[Cramer-Rao lower bound]], [[Score function]], [[Fisher information]].
