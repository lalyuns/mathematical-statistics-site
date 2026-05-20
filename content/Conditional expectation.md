---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Expectation]]"
tags:
  - statistics
  - conditional-expectation
source:
  - "[[Topic 2 revised]]"
pages:
  - Topic 2_revised_page_012.png
  - Topic 2_revised_page_013.png
---

# Conditional expectation

[[Conditional expectation]] $E[Y\mid X]$ is the best mean-square prediction of $Y$ using $X$.

It satisfies the tower property:

$$
E[E[Y\mid X]]=E[Y].
$$

The key algebraic rule is that known functions of $X$ can be pulled out:

$$
E[g(X)Y\mid X]=g(X)E[Y\mid X].
$$

Taking expectation again gives

$$
E[g(X)Y]=E[g(X)E[Y\mid X]].
$$

This is why, in Topic 2, the identity

$$
\operatorname{Cov}(X,Y)=\operatorname{Cov}(X,E[Y\mid X])
$$

follows by replacing $E[XY]$ with $E[XE(Y\mid X)]$.

## Projection view

Conditional expectation is the $L^2$ projection of $Y$ onto functions of $X$. For every candidate predictor $g(X)$,

$$
E[(Y-g(X))^2\mid X=x]
=E[Y^2\mid X=x]-2g(x)E[Y\mid X=x]+g(x)^2,
$$

which is minimized at

$$
g(x)=E[Y\mid X=x].
$$

Thus $E[Y\mid X]$ is not just a formula; it is the least-squares best prediction of $Y$ using the information in $X$.

Related: [[Law of total expectation]], [[Law of total variance]], [[Rao-Blackwell theorem]].
