---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - bayesian
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_008.png
  - Topic 4_revised_page_012.png
---

# Posterior distribution

The [[Posterior distribution]] updates a prior distribution using the observed sample.

If $\pi(\theta)$ is the prior and $f_X(x\mid\theta)$ is the sampling density, then

$$
\pi(\theta\mid x)
=\frac{f_X(x\mid\theta)\pi(\theta)}{m(x)},
\qquad
m(x)=\int f_X(x\mid\theta)\pi(\theta)\,d\theta.
$$

The denominator $m(x)$ is the marginal density of the data. It normalizes the posterior so that it integrates to one.

Bayes estimators minimize posterior expected loss under this distribution.

Related: [[Bayes estimator]], [[Conjugate prior]], [[Bayes rule]].
