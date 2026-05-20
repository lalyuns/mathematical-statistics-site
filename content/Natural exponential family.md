---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - exponential-family
  - sufficiency
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_005.png
aliases:
  - Exponential family completeness
---

# Natural exponential family

A $k$-parameter natural exponential family has density of the form

$$
f(x\mid\theta)=
\exp\left(\sum_{j=1}^k \eta_j(\theta)T_j(x)+h(x)+c(\theta)\right).
$$

For an iid sample, the statistic

$$
\left(\sum_{i=1}^nT_1(X_i),\ldots,\sum_{i=1}^nT_k(X_i)\right)
$$

is sufficient by [[Factorization theorem]].

Under the full-rank/open-parameter conditions used in standard exponential-family theory, this statistic is also complete. Topic 4 uses this fact as the main engine for applying [[Lehmann-Scheffe theorem]].

Related: [[Completeness]], [[Sufficient statistic]], [[Lehmann-Scheffe theorem]].
