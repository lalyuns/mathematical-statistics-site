---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Convergence]]"
tags:
  - statistics
  - asymptotics
  - mgf
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_006.png
aliases:
  - Continuity theorem for MGFs
  - Moment generating function continuity theorem
  - MGF convergence theorem
---

# MGF continuity theorem

[[MGF continuity theorem]] lets moment generating functions prove convergence in distribution.

If $X_n$ has MGF $M_n(t)$ and $X$ has MGF $M(t)$, and

$$
M_n(t)\to M(t)
$$

for all $t$ in some open interval around $0$, then

$$
X_n\xrightarrow{d}X.
$$

The open interval condition matters because an MGF defined near $0$ uniquely determines the distribution.

## CLT role

In the MGF proof of [[Central limit theorem]], the standardized mean $Y_n$ has

$$
M_{Y_n}(t)\to e^{t^2/2}.
$$

Since $e^{t^2/2}$ is the MGF of $N(0,1)$, the theorem gives

$$
Y_n\xrightarrow{d}N(0,1).
$$

Related: [[Moment generating function]], [[Convergence in distribution]], [[Central limit theorem]].
