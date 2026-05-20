---
created: 2026-05-21
aliases:
  - MP test
  - 最強力檢定是在固定 level 下最大化對立點的 power
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - hypothesis-tests
  - proofs
source:
  - "[[Topic 5 revised]]"
---

# Most powerful test

A [[Most powerful test]] maximizes [[Power]] at a fixed alternative point among all tests with the same level constraint.

For simple hypotheses, $\varphi$ is most powerful level $\alpha$ if every other [[Level alpha test]] $\psi$ satisfies

$$E_{\theta_A}[\varphi(X)]\ge E_{\theta_A}[\psi(X)].$$

[[Neyman-Pearson lemma]] proves that the LR test has this property.