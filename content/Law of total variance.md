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
aliases:
  - Variance decomposition
  - Conditional variance formula
  - 全變異公式
---

# Law of total variance

[[Law of total variance]] says

$$
\operatorname{Var}(Y)=E[\operatorname{Var}(Y\mid X)]
+\operatorname{Var}(E[Y\mid X]).
$$

Equivalently,

$$
\operatorname{Var}(Y-E[Y\mid X])=E[\operatorname{Var}(Y\mid X)].
$$

## Proof

Let

$$
m(X)=E[Y\mid X].
$$

Decompose the centered variable into a predictable part and a residual:

$$
Y-EY=(Y-m(X))+(m(X)-EY).
$$

When the square is expanded, the cross term vanishes:

$$
\begin{aligned}
E[(Y-m(X))(m(X)-EY)]
&=E\{E[(Y-m(X))(m(X)-EY)\mid X]\}\\
&=E\{(m(X)-EY)E[Y-m(X)\mid X]\}\\
&=0.
\end{aligned}
$$

The last line uses $E[Y-m(X)\mid X]=E[Y\mid X]-m(X)=0$.

Therefore

$$
\operatorname{Var}(Y)
=E[(Y-m(X))^2]+E[(m(X)-EY)^2].
$$

The first term is

$$
\begin{aligned}
E[(Y-m(X))^2]
&=E\{E[(Y-m(X))^2\mid X]\}\\
&=E[\operatorname{Var}(Y\mid X)],
\end{aligned}
$$

and the second term is

$$
E[(m(X)-EY)^2]=\operatorname{Var}(E[Y\mid X]).
$$

Combining the two terms proves the formula.

## Random-sum pattern

For a random sum $T=\sum_{i=1}^N X_i$ with $X_i$ iid, independent of $N$, mean $\mu$, and variance $\sigma^2$,

$$
E(T\mid N)=N\mu,\qquad \operatorname{Var}(T\mid N)=N\sigma^2.
$$

Then

$$
\operatorname{Var}(T)
=E[N\sigma^2]+\operatorname{Var}(N\mu)
=\sigma^2E[N]+\mu^2\operatorname{Var}(N).
$$

Related: [[Conditional expectation]], [[Law of total expectation]], [[Rao-Blackwell theorem]], [[Midterm problem - random sum mean and variance]].
