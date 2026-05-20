---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Joint distributions]]"
tags:
  - statistics
  - order-statistics
source:
  - "[[Topic 2 revised]]"
---

# Order statistics

For iid observations with CDF $F$ and PDF $f$, the $k$th order statistic has density

$$
f_{X_{(k)}}(x)=
\frac{n!}{(k-1)!(n-k)!}
[F(x)]^{k-1}[1-F(x)]^{n-k}f(x).
$$

The joint density of $X_{(i)}$ and $X_{(j)}$ partitions the sample into five regions around $u<v$.

Related: [[Midterm problem - order statistic densities]].
