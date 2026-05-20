---
created: 2026-05-21
categories:
  - Problems
topics:
  - Probability
tags:
  - statistics
  - midterm
  - conditional-probability
source:
  - "[[Topic 1 revised]]"
pages:
  - Test2_1_page_001.png
aliases:
  - Bayes rule from a partition
---

# Midterm problem - Bayes rule proof

## Restatement

Let $A_1,\ldots,A_n$ be a partition of the sample space with $P(A_i)>0$, and let $P(B)>0$. Prove [[Bayes rule]]:

$$
P(A_i\mid B)=
\frac{P(B\mid A_i)P(A_i)}
{\sum_{j=1}^n P(B\mid A_j)P(A_j)}.
$$

## Solution

Start from [[Conditional distribution|conditional probability]]:

$$
P(A_i\mid B)=\frac{P(A_i\cap B)}{P(B)}
=\frac{P(B\mid A_i)P(A_i)}{P(B)}.
$$

Because the $A_j$ form a partition,

$$
B=\bigcup_{j=1}^n (B\cap A_j)
$$

as a disjoint union. By additivity,

$$
P(B)=\sum_{j=1}^n P(B\cap A_j)
=\sum_{j=1}^n P(B\mid A_j)P(A_j).
$$

Substituting this denominator gives Bayes rule.

## Linked knowledge

- [[Bayes rule]]
- [[Probability function]]
- [[Conditional distribution]]

