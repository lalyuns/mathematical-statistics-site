---
created: 2026-05-20
aliases:
  - Wilks theorem 讓 LRT 有卡方近似分配
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - asymptotics
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_005.png"
---

# Wilks theorem

Under regularity conditions,

$$-2\log\lambda(X)\xrightarrow{d}\chi^2_{\dim(\Theta)-\dim(\Theta_0)}$$

under $H_0$.

[[Wilks theorem]] turns [[Likelihood ratio test]] into a general [[Asymptotic test]]. Large $-2\log\lambda$ rejects the null. The degrees of freedom are the dimension lost by imposing the null restriction.

Related: [[Multinomial LRT]], [[Normal mean LRT with unknown variance]].