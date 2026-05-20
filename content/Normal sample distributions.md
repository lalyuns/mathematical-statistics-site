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

# Normal sample distributions

If $X_i\overset{iid}{\sim}N(\mu,\sigma^2)$, then

$$
\bar X\sim N\left(\mu,\frac{\sigma^2}{n}\right),
\qquad
\frac{(n-1)S^2}{\sigma^2}\sim\chi^2_{n-1},
$$

and $\bar X$ is independent of $S^2$.

These facts produce the [[t distribution]] used in [[t confidence interval]].

For the proof skeleton with the missing MGF and orthogonal-decomposition steps filled in, see [[Normal sample theorem]].
