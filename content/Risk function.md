---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - bayesian
  - estimation
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_008.png
---

# Risk function

Given a loss function $L(\theta,\delta(X))$, the [[Risk function]] of an estimator $\delta$ is

$$
R(\theta,\delta)=E_\theta[L(\theta,\delta(X))].
$$

It is a function of the true parameter $\theta$ because the sampling distribution of $X$ depends on $\theta$.

In Bayesian estimation, the Bayes risk averages this risk over the prior:

$$
r(\delta)=\int R(\theta,\delta)\pi(\theta)\,d\theta.
$$

A [[Bayes estimator]] minimizes Bayes risk, equivalently posterior risk pointwise in the observed data.

Related: [[Bayes estimator]], [[Posterior distribution]], [[Bias variance MSE decomposition]].
