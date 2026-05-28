---
created: 2026-05-20
aliases:
  - 常態平均數的 t 信賴區間可以看成反轉 t 檢定
categories:
  - "[[Evergreen]]"
topics:
  - "[[Confidence set]]"
tags:
  - statistics
  - confidence-sets
  - normal-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_008.png"
---

# t confidence interval

The two-sided t interval for a normal mean with unknown variance is [[Test inversion]] of the t test.

The acceptance region

$$\left|\frac{\bar X_n-\mu_0}{S_n/\sqrt n}\right|\le t_{n-1,1-\alpha/2}$$

inverts to

$$\mu\in\left[\bar X_n-\frac{S_n}{\sqrt n}t_{n-1,1-\alpha/2},\ \bar X_n+\frac{S_n}{\sqrt n}t_{n-1,1-\alpha/2}\right].$$

For the one-sided alternative

$$
H_0:\mu=\mu_0,\qquad H_A:\mu<\mu_0,
$$

the acceptance region is

$$
A(\mu_0)=
\left\{
X:\frac{\bar X_n-\mu_0}{S_n/\sqrt n}\ge t_{n-1,\alpha}
\right\},
$$

and test inversion gives

$$
C(X)=
\left\{
\mu:\mu\in
\left(-\infty,\bar X_n-\frac{S_n}{\sqrt n}t_{n-1,\alpha}\right]
\right\}.
$$

For the one-sided alternative

$$
H_0:\mu=\mu_0,\qquad H_A:\mu>\mu_0,
$$

the acceptance region is

$$
A(\mu_0)=
\left\{
X:\frac{\bar X_n-\mu_0}{S_n/\sqrt n}\le t_{n-1,1-\alpha}
\right\},
$$

and test inversion gives

$$
C(X)=
\left\{
\mu:\mu\in
\left[\bar X_n-\frac{S_n}{\sqrt n}t_{n-1,1-\alpha},\infty\right)
\right\}.
$$

Related: [[Normal mean LRT with unknown variance]], [[Confidence set]].
