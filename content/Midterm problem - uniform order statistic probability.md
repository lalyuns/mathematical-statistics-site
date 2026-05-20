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
  - Probability that V falls between sample min and max
---

# Midterm problem - uniform order statistic probability

## Restatement

Let $U_1,\ldots,U_n,V$ be iid $\operatorname{Uniform}(0,1)$. Find

$$
P(U_{(1)}<V<U_{(n)}),
$$

where $U_{(1)}$ and $U_{(n)}$ are the minimum and maximum of $U_1,\ldots,U_n$.

## Solution

Among the $n+1$ iid continuous observations

$$
U_1,\ldots,U_n,V,
$$

all ranks are equally likely for $V$. The event $U_{(1)}<V<U_{(n)}$ means $V$ is neither the smallest nor the largest among all $n+1$ observations.

Thus

$$
P(U_{(1)}<V<U_{(n)})
=1-\frac{2}{n+1}
=\frac{n-1}{n+1}.
$$

## Linked knowledge

- [[Order statistics]]
- [[Independence]]
- [[Common distributions]]

