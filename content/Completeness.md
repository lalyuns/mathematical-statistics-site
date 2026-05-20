---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - sufficiency
  - estimation
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_005.png
aliases:
  - Complete statistic
---

# Completeness

A statistic $S$ is complete if every measurable function $g$ satisfying

$$
E_\theta[g(S)]=0\quad\text{for all }\theta
$$

must also satisfy

$$
P_\theta(g(S)=0)=1\quad\text{for all }\theta.
$$

Completeness says there are no nontrivial unbiased estimators of zero that are functions of $S$.

In [[Lehmann-Scheffe theorem]], this is what turns a sufficient statistic into a unique UMVUE-producing statistic.

Related: [[Sufficient statistic]], [[Lehmann-Scheffe theorem]], [[Natural exponential family]].
