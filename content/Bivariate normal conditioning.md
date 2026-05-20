---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Sampling distributions]]"
tags:
  - statistics
  - normal-theory
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_007.png
aliases:
  - Conditional distribution in a bivariate normal
---

# Bivariate normal conditioning

If $(X,Y)$ is bivariate normal with means $\mu_X,\mu_Y$, variances $\sigma_X^2,\sigma_Y^2$, and correlation $\rho$, then the conditional distribution of $X$ given $Y=y$ is normal:

$$
X\mid Y=y\sim
N\left(\mu_X+\rho\frac{\sigma_X}{\sigma_Y}(y-\mu_Y),
(1-\rho^2)\sigma_X^2\right).
$$

The conditional mean is linear in the observed value $y$, and the conditional variance does not depend on $y$.

This is a special case where [[Conditional expectation]] becomes a linear regression formula:

$$
E[X\mid Y]=\mu_X+\rho\frac{\sigma_X}{\sigma_Y}(Y-\mu_Y).
$$

Related: [[Normal sample distributions]], [[Conditional distribution]], [[Conditional expectation]].
