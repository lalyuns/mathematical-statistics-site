---
created: 2026-05-21
categories:
  - Problems
topics:
  - Expectation
tags:
  - statistics
  - midterm
  - conditional-expectation
source:
  - "[[Topic 2 revised]]"
pages:
  - test1_page_020.png
aliases:
  - Covariance and conditional expectation identities
---

# Midterm problem - conditional covariance identities

## Restatement

Prove the conditional expectation identities

$$
\operatorname{Cov}(X,Y)=\operatorname{Cov}(X,E(Y\mid X))
$$

and

$$
\operatorname{Var}(Y-E(Y\mid X))=E(\operatorname{Var}(Y\mid X)).
$$

## Solution

For the covariance identity, use the tower property:

$$
E(Y)=E(E(Y\mid X)).
$$

Also,

$$
E(XY)=E(E(XY\mid X))=E(XE(Y\mid X)).
$$

Therefore

$$
\operatorname{Cov}(X,Y)
=E(XY)-E(X)E(Y)
=E(XE(Y\mid X))-E(X)E(E(Y\mid X)),
$$

which equals $\operatorname{Cov}(X,E(Y\mid X))$.

For the variance identity, let $m(X)=E(Y\mid X)$. Since

$$
E(Y-m(X)\mid X)=0,
$$

we get

$$
\operatorname{Var}(Y-m(X))
=E((Y-m(X))^2)
=E(E((Y-m(X))^2\mid X)).
$$

The inner term is $\operatorname{Var}(Y\mid X)$, so

$$
\operatorname{Var}(Y-E(Y\mid X))=E(\operatorname{Var}(Y\mid X)).
$$

## Linked knowledge

- [[Conditional expectation]]
- [[Law of total expectation]]
- [[Law of total variance]]
- [[Expectation]]
