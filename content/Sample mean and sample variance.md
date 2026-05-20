---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Sampling distributions]]"
tags:
  - statistics
  - sampling
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_002.png
aliases:
  - Sample mean
  - Sample variance
---

# Sample mean and sample variance

For a [[Random sample]] $X_1,\ldots,X_n$ with mean $\mu$ and variance $\sigma^2$,

$$
\bar X=\frac1n\sum_{i=1}^n X_i,
\qquad
S^2=\frac{1}{n-1}\sum_{i=1}^n(X_i-\bar X)^2.
$$

The sample mean is unbiased and has variance

$$
E[\bar X]=\mu,\qquad \operatorname{Var}(\bar X)=\frac{\sigma^2}{n}.
$$

The sample variance is unbiased:

$$
E[S^2]=\sigma^2.
$$

## Proof of unbiased sample variance

Use the identity

$$
\sum_{i=1}^n(X_i-\bar X)^2=\sum_{i=1}^nX_i^2-n\bar X^2.
$$

Then

$$
\begin{aligned}
E[S^2]
&=\frac{1}{n-1}\left(nE[X_1^2]-nE[\bar X^2]\right)\\
&=\frac{1}{n-1}\left(n(\mu^2+\sigma^2)-n\left(\mu^2+\frac{\sigma^2}{n}\right)\right)\\
&=\sigma^2.
\end{aligned}
$$

Related: [[Random sample]], [[Normal sample distributions]], [[Weak law of large numbers]].
