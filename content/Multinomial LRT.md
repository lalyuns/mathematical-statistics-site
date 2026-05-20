---
created: 2026-05-20
aliases:
  - 多項分配的 LRT 會導向 Pearson 卡方統計量
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - chi-square-tests
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_005.png"
  - "page_006.png"
---

# Multinomial LRT

For multinomial data, the LR deviance is

$$-2\log\lambda=2\sum_{j=1}^m O_j\log\left(\frac{O_j}{E_j}\right).$$

A Taylor expansion gives Pearson's chi-square statistic:

$$\sum_{j=1}^m\frac{(O_j-E_j)^2}{E_j}.$$

This is [[Wilks theorem]] in the multinomial goodness-of-fit setting.

For the missing Taylor steps, see [[Pearson chi-square approximation]].
