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
pages:
  - Topic 3_revised_page_005.png
aliases:
  - SLLN
---

# Strong law of large numbers

The [[Strong law of large numbers]] says that for iid $X_1,X_2,\ldots$ with mean $\mu$,

$$
\bar X_n\xrightarrow{a.s.}\mu.
$$

It strengthens the [[Weak law of large numbers]], which only gives convergence in probability.

In Monte Carlo integration, if $X_i\overset{iid}{\sim}U(0,1)$, then

$$
\frac1n\sum_{i=1}^n f(X_i)\xrightarrow{a.s.}\int_0^1 f(x)\,dx.
$$

This is the theoretical reason sample averages approximate integrals.

Related: [[Convergence almost surely]], [[Weak law of large numbers]], [[Convergence in probability]].
