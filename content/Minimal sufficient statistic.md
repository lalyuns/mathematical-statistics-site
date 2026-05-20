---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - sufficiency
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_004.png
---

# Minimal sufficient statistic

A [[Minimal sufficient statistic]] is a sufficient statistic that is a function of every other sufficient statistic.

If $S$ is minimal sufficient and $S^*$ is sufficient, then there is a function $r$ such that

$$
S=r(S^*).
$$

So $S$ is the coarsest data reduction that still preserves all information about $\theta$.

Minimal sufficiency is about not keeping unnecessary information. [[Completeness]] is a different property: it prevents nonzero functions of the statistic from having expectation zero for all $\theta$.

Related: [[Sufficient statistic]], [[Factorization theorem]], [[Completeness]].
