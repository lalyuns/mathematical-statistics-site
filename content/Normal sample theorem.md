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
  - Topic 3_revised_page_002.png
  - Topic 3_revised_page_003.png
aliases:
  - Normal sample theory
---

# Normal sample theorem

If

$$
X_1,\ldots,X_n\overset{iid}{\sim}N(\mu,\sigma^2),
$$

then

$$
\bar X\sim N\left(\mu,\frac{\sigma^2}{n}\right),
\qquad
\frac{(n-1)S^2}{\sigma^2}\sim\chi^2_{n-1},
$$

and $\bar X$ is independent of $S^2$.

## Proof idea from Topic 3

The lecture proves independence by looking at the joint MGF of

$$
\bar X,\quad X_1-\bar X,\ldots,X_n-\bar X.
$$

The MGF factors into a term involving only $\bar X$ and terms involving only the residuals. This shows

$$
\bar X\perp (X_1-\bar X,\ldots,X_n-\bar X).
$$

Since $S^2$ is a function of the residual vector, $\bar X$ is independent of $S^2$.

For the chi-square result, use the orthogonal decomposition

$$
\sum_{i=1}^n\left(\frac{X_i-\mu}{\sigma}\right)^2
=
\sum_{i=1}^n\left(\frac{X_i-\bar X}{\sigma}\right)^2
+
\left(\frac{\bar X-\mu}{\sigma/\sqrt n}\right)^2.
$$

The left side is $\chi^2_n$ and the last term is $\chi^2_1$, independent of the residual term. Therefore the residual term is $\chi^2_{n-1}$.

Related: [[Normal sample distributions]], [[Chi-square distribution]], [[Studentized sample mean]].
