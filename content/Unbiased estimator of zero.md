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
  - Topic 4_revised_page_005.png
---

# Unbiased estimator of zero

An [[Unbiased estimator of zero]] is a statistic $U(X)$ such that

$$
E_\theta[U(X)]=0
$$

for every $\theta$ in the parameter space.

These statistics measure directions in which one unbiased estimator can be perturbed while staying unbiased:

$$
W+aU
$$

is unbiased for the same target as $W$ whenever $W$ is unbiased for that target.

This is the hidden object in the [[UMVUE characterization]] and the proof of [[Lehmann-Scheffe theorem]].

Related: [[UMVUE characterization]], [[Completeness]], [[Lehmann-Scheffe theorem]].
