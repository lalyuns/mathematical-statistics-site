---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - likelihood-ratio-tests
  - sufficiency
source:
  - "[[Topic 5 revised]]"
pages:
  - page_003.png
aliases:
  - Likelihood ratio based on sufficient statistic
---

# LRT depends on sufficient statistic

If $S(X)$ is sufficient and the likelihood factors as

$$
L(\theta\mid x)=g_\theta(S(x))h(x),
$$

then the [[Likelihood ratio statistic]] can be computed from $S(X)$ alone:

$$
\lambda(x)
=\frac{\sup_{\theta\in\Theta_0}g_\theta(S(x))h(x)}
{\sup_{\theta\in\Theta}g_\theta(S(x))h(x)}
=\frac{\sup_{\theta\in\Theta_0}g_\theta(S(x))}
{\sup_{\theta\in\Theta}g_\theta(S(x))}.
$$

The factor $h(x)$ cancels because it does not depend on $\theta$.

This proves the Topic 5 remark that the LRT statistic based on the full sample equals the LRT statistic based on a sufficient statistic.

Related: [[Likelihood ratio statistic]], [[Factorization theorem]], [[Sufficient statistic]].
