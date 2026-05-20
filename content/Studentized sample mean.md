---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Sampling distributions]]"
tags:
  - statistics
  - normal-theory
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_003.png
aliases:
  - Studentized mean
  - t statistic for a normal mean
---

# Studentized sample mean

For a normal sample with unknown variance, the standardized sample mean with $\sigma$ replaced by $S$ is

$$
T=\frac{\sqrt n(\bar X-\mu)}{S}.
$$

By [[Normal sample theorem]],

$$
Z=\frac{\sqrt n(\bar X-\mu)}{\sigma}\sim N(0,1),
\qquad
U=\frac{(n-1)S^2}{\sigma^2}\sim\chi^2_{n-1},
$$

with $Z\perp U$. Hence

$$
T=\frac{Z}{\sqrt{U/(n-1)}}\sim t_{n-1}.
$$

This statistic is the exact pivot behind the one-sample [[t confidence interval]] and exact t tests.

Related: [[t distribution]], [[Normal sample distributions]], [[Exact test]].
