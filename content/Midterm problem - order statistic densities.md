---
created: 2026-05-21
categories:
  - Problems
topics:
  - Joint distributions
tags:
  - statistics
  - midterm
  - order-statistics
source:
  - "[[Topic 2 revised]]"
pages:
  - Test2_2_page_001.png
aliases:
  - Joint density of two order statistics
---

# Midterm problem - order statistic densities

## Restatement

For a continuous iid sample with CDF $F$ and density $f$, find the joint density of $X_{(i)}$ and $X_{(j)}$ for $i<j$. Then specialize to the minimum and maximum of a uniform sample.

## Solution

For $u<v$,

$$
\begin{aligned}
f_{X_{(i)},X_{(j)}}(u,v)
&=\frac{n!}{(i-1)!(j-i-1)!(n-j)!}\\
&\quad\times [F(u)]^{i-1}[F(v)-F(u)]^{j-i-1}[1-F(v)]^{n-j}f(u)f(v).
\end{aligned}
$$

The factors correspond to:

- $i-1$ observations below $u$,
- $j-i-1$ observations between $u$ and $v$,
- $n-j$ observations above $v$,
- one observation near $u$ and one near $v$.

For iid $\operatorname{Uniform}(0,1)$, the joint density of the minimum $U$ and maximum $V$ is

$$
f_{U,V}(u,v)=n(n-1)(v-u)^{n-2},\qquad 0<u<v<1.
$$

Useful moments are

$$
E(U)=\frac{1}{n+1},\qquad E(V)=\frac{n}{n+1},
$$

and

$$
\operatorname{Var}(U)=\operatorname{Var}(V)=
\frac{n}{(n+1)^2(n+2)}.
$$

## Linked knowledge

- [[Order statistics]]
- [[Joint distribution]]
- [[Expectation]]

