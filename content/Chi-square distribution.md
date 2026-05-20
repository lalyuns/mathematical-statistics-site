---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Sampling distributions]]"
tags:
  - statistics
  - normal-theory
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_002.png
  - Topic 3_revised_page_003.png
---

# Chi-square distribution

A chi-square random variable with $k$ degrees of freedom is the sum of squares of $k$ independent standard normal variables:

$$
U=\sum_{i=1}^k Z_i^2,\qquad Z_i\overset{iid}{\sim}N(0,1).
$$

Then

$$
U\sim\chi^2_k.
$$

Equivalently,

$$
\chi^2_k\sim \operatorname{Gamma}\left(\frac{k}{2},\frac12\right)
$$

under the shape-rate convention used by the lecture.

In normal sample theory,

$$
\frac{(n-1)S^2}{\sigma^2}\sim\chi^2_{n-1}.
$$

Related: [[Normal sample distributions]], [[t distribution]], [[F distribution]].
