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
aliases:
  - Tower property
  - Iterated expectation
  - Law of iterated expectation
  - 全期望公式
---

# Law of total expectation

[[Law of total expectation]] says that averaging a conditional mean gives the original mean:

$$
E[E(Y\mid X)]=E(Y).
$$

More generally, if $Z$ contains at least as much information as $X$, then

$$
E[E(Y\mid Z)\mid X]=E(Y\mid X).
$$

This is also called the tower property.

## Proof for the discrete case

Start from the definition

$$
E(Y\mid X=x)=\sum_y y\,P(Y=y\mid X=x).
$$

Then

$$
\begin{aligned}
E[E(Y\mid X)]
&=\sum_x E(Y\mid X=x)P(X=x)\\
&=\sum_x\sum_y y\,P(Y=y\mid X=x)P(X=x)\\
&=\sum_x\sum_y y\,P(X=x,Y=y)\\
&=\sum_y y\sum_x P(X=x,Y=y)\\
&=\sum_y y\,P(Y=y)\\
&=E(Y).
\end{aligned}
$$

The continuous proof is the same calculation with sums replaced by integrals and $f_{Y\mid X}(y\mid x)f_X(x)=f_{X,Y}(x,y)$.

## Useful forms

If $g(X)$ is a function of the conditioning variable, it can be pulled outside the inner conditional expectation:

$$
E[g(X)Y\mid X]=g(X)E(Y\mid X).
$$

Therefore

$$
E[g(X)Y]=E[g(X)E(Y\mid X)].
$$

This identity is the workhorse behind covariance decompositions, random-sum formulas, [[Rao-Blackwell theorem]], and [[Law of total variance]].

Related: [[Conditional expectation]], [[Expectation]], [[Law of total variance]].
