---
created: 2026-05-21
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
  - page_006.png
aliases:
  - Pearson chi-square statistic
---

# Pearson chi-square approximation

The likelihood-ratio deviance for multinomial counts often has the form

$$
2\sum_{j=1}^m O_j\log\left(\frac{O_j}{E_j}\right).
$$

When $O_j$ is close to $E_j$, set $O_j=E_j+d_j$. Taylor expand

$$
\log\left(1+\frac{d_j}{E_j}\right)
=\frac{d_j}{E_j}-\frac{d_j^2}{2E_j^2}+o(d_j^2/E_j^2).
$$

Then

$$
2O_j\log\left(\frac{O_j}{E_j}\right)
\approx 2(E_j+d_j)\left(\frac{d_j}{E_j}-\frac{d_j^2}{2E_j^2}\right)
\approx 2d_j+\frac{d_j^2}{E_j}.
$$

In multinomial goodness-of-fit problems, the linear terms sum to zero because total observed and expected counts agree:

$$
\sum_j d_j=\sum_j(O_j-E_j)=0.
$$

So the deviance is approximated by Pearson's statistic:

$$
\sum_{j=1}^m\frac{(O_j-E_j)^2}{E_j}.
$$

The degrees of freedom subtract the number of estimated parameters and the total-count constraint.

Related: [[Multinomial LRT]], [[Wilks theorem]], [[Likelihood ratio test]].
