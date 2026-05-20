---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Expectation]]"
tags:
  - statistics
  - expectation
source:
  - "[[Topic 2 revised]]"
---

# Tail integral formula

For nonnegative continuous $X$ with finite mean,

$$
E[X]=\int_0^\infty P(X>t)\,dt
=\int_0^\infty (1-F_X(t))\,dt.
$$

This follows by writing $x=\int_0^x dt$ and switching the order of integration.
