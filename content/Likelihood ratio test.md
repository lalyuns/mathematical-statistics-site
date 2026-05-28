---
created: 2026-05-20
aliases:
  - LRT
  - Likelihood ratio test 用小概似比作為拒絕證據
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_003.png"
---

# Likelihood ratio test

[[Likelihood ratio test]] rejects small [[Likelihood ratio statistic|likelihood ratios]] because the restricted model fits poorly relative to the full model.

A size $\alpha$ LRT uses

$$\varphi(x)=1(\lambda(x)<\lambda^*)+\gamma 1(\lambda(x)=\lambda^*).$$

The lecture writes the boundary randomization as

$$
\varphi(x)=I(\lambda(x)<\lambda^*)
+\frac{\alpha-\alpha_\ell}{\alpha_u-\alpha_\ell}I(\lambda(x)=\lambda^*),
$$

where

$$
\sup_{\theta\in\Theta_0}P_\theta(\lambda(X)<\lambda^*)=\alpha_\ell\le\alpha
$$

and

$$
\sup_{\theta\in\Theta_0}P_\theta(\lambda(X)\le\lambda^*)=\alpha_u\ge\alpha.
$$

The convention $0/0=0$ is used if the boundary has no null probability.

The boundary term $\gamma$ is [[Boundary randomization]]. For simple hypotheses, LRT is justified by [[Neyman-Pearson lemma]].
