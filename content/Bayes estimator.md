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
  - Topic 4_revised_page_009.png
---

# Bayes estimator

A [[Bayes estimator]] minimizes posterior risk.

Under squared error loss, it is the posterior mean. Under absolute error loss, it is a posterior median.

The Bayes-risk minimization can be rewritten pointwise in the observed data:

$$
\int R(\theta,\delta)\pi(\theta)\,d\theta
=\int \left[\int L(\theta,\delta(x))\pi(\theta\mid x)\,d\theta\right]m(x)\,dx.
$$

Since $m(x)\ge0$, minimizing Bayes risk reduces to minimizing the posterior risk

$$
\int L(\theta,\delta(x))\pi(\theta\mid x)\,d\theta
$$

for each observed $x$.

Related: [[Posterior distribution]], [[Risk function]], [[Bayes rule]], [[Conjugate prior]].
