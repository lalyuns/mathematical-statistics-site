---
created: 2026-05-21
categories:
  - Problems
topics:
  - Sampling distributions
tags:
  - statistics
  - midterm
  - normal-theory
source:
  - "[[Topic 3 revised]]"
pages:
  - Test2_3_page_001.png
aliases:
  - Exact normal sample distributions
---

# Midterm problem - normal sample exact distributions

## Restatement

For a random sample from $N(\mu,\sigma^2)$, derive the exact distributions used for inference on $\mu$ and $\sigma^2$.

## Solution

If $X_1,\ldots,X_n\sim N(\mu,\sigma^2)$ iid, then

$$
\bar X\sim N\left(\mu,\frac{\sigma^2}{n}\right).
$$

The standardized mean is

$$
Z=\frac{\bar X-\mu}{\sigma/\sqrt n}\sim N(0,1).
$$

The sample variance satisfies

$$
\frac{(n-1)S^2}{\sigma^2}\sim \chi^2_{n-1}.
$$

Also, $\bar X$ and $S^2$ are independent. Therefore

$$
T=\frac{\bar X-\mu}{S/\sqrt n}\sim t_{n-1}.
$$

For two independent normal samples, the ratio of scaled sample variances follows an [[F distribution]]:

$$
\frac{S_1^2/\sigma_1^2}{S_2^2/\sigma_2^2}\sim F_{n_1-1,n_2-1}.
$$

## Linked knowledge

- [[Normal sample distributions]]
- [[Sampling distribution]]
- [[t distribution]]
- [[F distribution]]
- [[Quiz problem - exact t statistic]]

