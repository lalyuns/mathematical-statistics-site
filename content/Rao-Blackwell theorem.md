---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - estimation
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_004.png
  - Topic 4_revised_page_005.png
---

# Rao-Blackwell theorem

If $W$ is unbiased for $\tau(\theta)$ and $S$ is sufficient, then

$$
\phi(S)=E[W\mid S]
$$

is unbiased and has variance no larger than $W$.

Rao-Blackwellization improves estimators by conditioning on sufficient information.

## Proof ingredients

Unbiasedness follows by [[Law of total expectation]]:

$$
E_\theta[\phi(S)]
=E_\theta[E_\theta(W\mid S)]
=E_\theta[W]
=\tau(\theta).
$$

The variance improvement follows by [[Law of total variance]]:

$$
\operatorname{Var}_\theta(W)
=\operatorname{Var}_\theta(E_\theta[W\mid S])
+E_\theta[\operatorname{Var}_\theta(W\mid S)]
\ge \operatorname{Var}_\theta(\phi(S)).
$$

Sufficiency matters because it makes $\phi(S)$ a statistic whose definition does not depend on the unknown parameter.

Related: [[Conditional expectation]], [[Law of total expectation]], [[Law of total variance]], [[UMVUE]].
