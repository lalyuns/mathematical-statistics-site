---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Convergence]]"
tags:
  - statistics
  - asymptotics
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_007.png
aliases:
  - Slutsky's theorem
---

# Slutsky theorem

[[Slutsky theorem]] combines convergence in distribution with convergence in probability to a constant.

If

$$
X_n\xrightarrow{d}X,\qquad Y_n\xrightarrow{p}c,
$$

then

$$
X_n+Y_n\xrightarrow{d}X+c,
\qquad
X_nY_n\xrightarrow{d}cX.
$$

It is the step that lets asymptotic proofs replace a random normalizing matrix by its probability limit.

In Topic 4, it is used after the MLE score expansion:

$$
\frac{1}{\sqrt n}S(\theta_0)
-\left(\frac1n I(\theta^*)\right)\sqrt n(\hat\theta-\theta_0)=0.
$$

The first term has a CLT limit, and the observed information term converges in probability to Fisher information.

Related: [[Convergence in distribution]], [[Convergence in probability]], [[Asymptotic normality of MLE]].
