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

# Factorization theorem

[[Factorization theorem]] says that $S(X)$ is sufficient if the joint density can be written as

$$
f_X(x\mid\theta)=g_\theta(S(x))h(x).
$$

It is the main practical test for [[Sufficient statistic]].

## Why the factorization proves sufficiency

In the discrete case, condition on $S(X)=s$:

$$
P_\theta(X=x\mid S(X)=s)
=\frac{P_\theta(X=x)}{P_\theta(S(X)=s)}
$$

when $S(x)=s$, and is $0$ otherwise. If

$$
P_\theta(X=x)=g_\theta(S(x))h(x),
$$

then

$$
P_\theta(S(X)=s)=\sum_{y:S(y)=s}g_\theta(s)h(y)
=g_\theta(s)\sum_{y:S(y)=s}h(y).
$$

So

$$
P_\theta(X=x\mid S(X)=s)
=\frac{h(x)}{\sum_{y:S(y)=s}h(y)},
$$

which no longer depends on $\theta$. That is exactly sufficiency.

Related: [[Sufficient statistic]], [[Minimal sufficient statistic]], [[Natural exponential family]].
