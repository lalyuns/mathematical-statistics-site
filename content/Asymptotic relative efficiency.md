---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - asymptotics
  - estimation
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_008.png
aliases:
  - ARE
---

# Asymptotic relative efficiency

Suppose two estimators satisfy

$$
\sqrt n(W_1-\tau(\theta))\xrightarrow{d}N(0,v_1(\theta)),
\qquad
\sqrt n(W_2-\tau(\theta))\xrightarrow{d}N(0,v_2(\theta)).
$$

The asymptotic relative efficiency of $W_1$ versus $W_2$ is

$$
ARE(W_1,W_2)=\frac{v_2(\theta)}{v_1(\theta)}.
$$

Large values favor $W_1$ because it has smaller asymptotic variance. This is the asymptotic analogue of comparing finite-sample variances of unbiased estimators.

Related: [[Asymptotic normality of MLE]], [[Cramer-Rao lower bound]], [[UMVUE]].
