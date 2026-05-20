---
created: 2026-05-20
aliases:
  - Poisson dispersion test 檢查多個 Poisson 平均是否相同
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - poisson-tests
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_006.png"
---

# Poisson dispersion test

[[Poisson dispersion test]] checks whether independent Poisson variables share one mean:

$$H_0:\lambda_1=\cdots=\lambda_n=\lambda.$$

The LR deviance is

$$2\sum_{i=1}^n X_i\log\left(\frac{X_i}{\bar X}\right).$$

A Taylor approximation gives

$$\frac{1}{\bar X}\sum_{i=1}^n(X_i-\bar X)^2\approx\chi^2_{n-1}.$$

Related: [[Likelihood ratio test]], [[Asymptotic test]].