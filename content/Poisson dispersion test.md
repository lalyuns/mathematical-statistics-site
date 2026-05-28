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

The likelihood-ratio statistic itself is

$$
\lambda(X_1,\ldots,X_n)
=
\prod_{i=1}^n
\left(\frac{\bar X}{X_i}\right)^{X_i}
e^{X_i-\bar X},
\qquad
\bar X=\frac1n\sum_{i=1}^nX_i.
$$

Therefore

$$
-2\log\lambda(X_1,\ldots,X_n)
=-2\sum_{i=1}^n
\left((X_i-\bar X)+X_i\log\frac{\bar X}{X_i}\right)
=2\sum_{i=1}^nX_i\log\frac{X_i}{\bar X}.
$$

A Taylor approximation gives

$$\frac{1}{\bar X}\sum_{i=1}^n(X_i-\bar X)^2\approx\chi^2_{n-1}.$$

The approximation is the same local quadratic idea as [[Pearson chi-square approximation]]: the likelihood deviance becomes a squared-deviation statistic near the null model.

Related: [[Likelihood ratio test]], [[Pearson chi-square approximation]], [[Asymptotic test]].
