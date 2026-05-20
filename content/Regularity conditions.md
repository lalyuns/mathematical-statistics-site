---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - estimation
  - likelihood
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_002.png
  - Topic 4_revised_page_007.png
---

# Regularity conditions

[[Regularity conditions]] are assumptions that justify exchanging limits, derivatives, integrals, and probability approximations in likelihood theory.

In Topic 4, the key uses are:

- differentiating $E_\theta[W(X)]$ under the integral sign,
- proving $E_\theta[\partial_\theta\log f(X\mid\theta)]=0$,
- replacing Fisher information by $-E_\theta[\partial_\theta^2\log f(X\mid\theta)]$,
- applying Taylor expansion to the likelihood score,
- using laws of large numbers on observed information.

A typical condition is the existence of an integrable dominating function $h_\theta(x)$ such that nearby second derivatives of $\log f(x\mid\theta)$ are bounded by $h_\theta(x)$. This is the technical reason the random Taylor remainder behaves well.

Related: [[Score function]], [[Fisher information]], [[Asymptotic normality of MLE]].
