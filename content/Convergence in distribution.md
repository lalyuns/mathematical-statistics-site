---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Convergence]]"
tags:
  - statistics
  - convergence
source:
  - "[[Topic 3 revised]]"
---

# Convergence in distribution

$X_n\xrightarrow{d}X$ if $F_n(x)\to F(x)$ at every continuity point of $F$.

This is the convergence used by [[Central limit theorem]], [[Asymptotic test]], and [[Wilks theorem]].

One practical proof route is [[MGF continuity theorem]]: show that the MGFs $M_{X_n}(t)$ converge to the MGF of the proposed limit on an interval around $0$.
