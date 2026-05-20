---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
tags:
  - statistics
  - quizzes
  - normal-tests
source:
  - "[[Quiz 2 hypothesis testing problems MOC]]"
pages:
  - "Test6_page_001.png"
---

# Quiz problem - exact t statistic

## Restatement

Let $X_1,\ldots,X_n\overset{iid}{\sim}N(\mu,\sigma^2)$, with both $\mu$ and $\sigma^2$ unknown.

Derive the sampling distributions of

$$
\bar X=\frac{1}{n}\sum_{i=1}^n X_i
$$

and

$$
S_n^2=\frac{1}{n-1}\sum_{i=1}^n(X_i-\bar X)^2,
$$

then derive the distribution of

$$
\frac{\sqrt n(\bar X-\mu)}{S_n}.
$$

## Solution

For a normal sample,

$$
\bar X\sim N\left(\mu,\frac{\sigma^2}{n}\right).
$$

Also,

$$
\frac{(n-1)S_n^2}{\sigma^2}\sim\chi^2_{n-1}.
$$

The sample mean and sample variance are independent:

$$
\bar X\perp S_n^2.
$$

Therefore

$$
\frac{\sqrt n(\bar X-\mu)}{S_n}
=
\frac{Z}{\sqrt{U/(n-1)}},
$$

where $Z\sim N(0,1)$, $U\sim\chi^2_{n-1}$, and $Z\perp U$.

Thus

$$
\frac{\sqrt n(\bar X-\mu)}{S_n}\sim t_{n-1}.
$$

This is the exact distribution behind the [[t confidence interval]].

## Links

- [[Exact test]]
- [[t confidence interval]]
- [[Test inversion]]
