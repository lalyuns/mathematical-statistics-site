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

The boundary term $\gamma$ is [[Boundary randomization]]. For simple hypotheses, LRT is justified by [[Neyman-Pearson lemma]].