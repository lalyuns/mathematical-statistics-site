---
created: 2026-05-21
aliases:
  - Level alpha test 把虛無假設下的拒絕機率限制在 alpha 以內
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
tags:
  - statistics
  - hypothesis-tests
  - proofs
source:
  - "[[Topic 5 revised]]"
---

# Level alpha test

A [[Level alpha test]] keeps the null-side rejection probability below $\alpha$:

$$\sup_{\theta\in\Theta_0}\beta(\theta)\le\alpha.$$

For a simple null $H_0:\theta=\theta_0$, this becomes $E_{\theta_0}[\varphi(X)]\le\alpha$.

[[Neyman-Pearson lemma]] compares all tests satisfying this constraint.