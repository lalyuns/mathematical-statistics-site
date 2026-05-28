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

For

$$
(X_1,\ldots,X_m)\sim\operatorname{Multinomial}(n,p_1,\ldots,p_m),
\qquad
\sum_{j=1}^mX_j=n,\quad \sum_{j=1}^mp_j=1,
$$

consider a parametric null model

$$
H_0:p_j=p_j(\theta),\ \theta\in\Theta_0,
\qquad
H_A:p_j\ne p_j(\theta).
$$

The likelihood-ratio statistic is

$$
\lambda(x_1,\ldots,x_m)
=
\prod_{j=1}^m
\left(\frac{p_j(\hat\theta)}{\hat p_j}\right)^{x_j},
\qquad
\hat p_j=\frac{x_j}{n},
$$

where $\hat\theta$ is the MLE inside the null parameter space $\Theta_0$.

For multinomial data, the LR deviance is

$$-2\log\lambda=2\sum_{j=1}^m O_j\log\left(\frac{O_j}{E_j}\right).$$

Here

$$
O_j=n\hat p_j=X_j,
\qquad
E_j=np_j(\hat\theta).
$$

A Taylor expansion gives Pearson's chi-square statistic:

$$\sum_{j=1}^m\frac{(O_j-E_j)^2}{E_j}.$$

Under the null, the limiting degrees of freedom are

$$
m-1-\dim(\Theta_0).
$$

This is [[Wilks theorem]] in the multinomial goodness-of-fit setting.

For the missing Taylor steps, see [[Pearson chi-square approximation]].
