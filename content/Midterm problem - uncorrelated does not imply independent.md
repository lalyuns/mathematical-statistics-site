---
created: 2026-05-21
categories:
  - Problems
topics:
  - Joint distributions
tags:
  - statistics
  - midterm
  - independence
source:
  - "[[Topic 2 revised]]"
pages:
  - test1_page_018.png
aliases:
  - Zero covariance without independence
---

# Midterm problem - uncorrelated does not imply independent

## Restatement

Give an example where $\operatorname{Cov}(X,Y)=0$ but $X$ and $Y$ are not independent. The test1 solution uses a uniform distribution on the unit disk.

## Solution

Let $(X,Y)$ be uniform on the unit disk

$$
x^2+y^2\leq 1.
$$

By symmetry,

$$
E(X)=0,\qquad E(Y)=0,\qquad E(XY)=0.
$$

Hence

$$
\operatorname{Cov}(X,Y)=E(XY)-E(X)E(Y)=0.
$$

But $X$ and $Y$ are not independent. The support is not a rectangle: if $X$ is close to $1$, then $Y$ must be close to $0$. For instance, conditioning on $X=x$ restricts $Y$ to

$$
-\sqrt{1-x^2}\leq Y\leq \sqrt{1-x^2},
$$

so the conditional range of $Y$ depends on $x$.

## Linked knowledge

- [[Independence]]
- [[Joint distribution]]
- [[Expectation]]

