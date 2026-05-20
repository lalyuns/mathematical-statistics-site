---
created: 2026-05-21
categories:
  - Problems
topics:
  - Probability
tags:
  - statistics
  - midterm
  - probability-inequalities
source:
  - "[[Topic 1 revised]]"
pages:
  - Test2_1_page_001.png
aliases:
  - Bonferroni lower bound for an intersection
---

# Midterm problem - Boole lower bound

## Restatement

Given events $A_1,\ldots,A_n$ in a [[Probability space]], prove

$$
P\left(\bigcap_{i=1}^n A_i\right)\geq \sum_{i=1}^n P(A_i)-(n-1).
$$

Then show that if $P(A_i)=1$ for every $i$, then $P(\cap_i A_i)=1$.

## Solution

Use [[Event|complements]] and [[Boole inequality]]:

$$
\begin{aligned}
P\left(\bigcap_{i=1}^n A_i\right)
&=1-P\left(\left(\bigcap_{i=1}^n A_i\right)^c\right)\\
&=1-P\left(\bigcup_{i=1}^n A_i^c\right)\\
&\geq 1-\sum_{i=1}^n P(A_i^c)\\
&=1-\sum_{i=1}^n (1-P(A_i))\\
&=\sum_{i=1}^n P(A_i)-(n-1).
\end{aligned}
$$

If $P(A_i)=1$ for all $i$, the lower bound becomes $1$. Since every probability is at most $1$, the intersection has probability exactly $1$.

## Linked knowledge

- [[Probability function]]
- [[Boole inequality]]
- [[Event]]

