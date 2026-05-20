---
created: 2026-05-20
aliases:
  - 未知變異數的常態平均數 LRT 會化成 t 檢定
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - normal-tests
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_005.png"
---

# Normal mean LRT with unknown variance

For $X_i\overset{iid}{\sim}N(\mu,\sigma^2)$ with unknown $\sigma^2$, test

$$H_0:\mu=\mu_0,\qquad H_A:\mu\ne\mu_0.$$

The [[Likelihood ratio test]] reduces to rejecting large

$$\left|\frac{\bar X_n-\mu_0}{S_n/\sqrt n}\right|.$$

Thus the exact LRT is the two-sided one-sample t test. A separate [[Asymptotic test]] uses [[Wilks theorem]] and $\chi^2_1$.

Related: [[t confidence interval]], [[Test inversion]].