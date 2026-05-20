---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Sampling distributions]]"
tags:
  - statistics
  - sampling
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_001.png
---

# Sampling without replacement

In [[Sampling without replacement]], observations are drawn from a finite population without returning selected units to the population.

For a finite population $\{x^{(1)},\ldots,x^{(N)}\}$, each draw has the same marginal distribution:

$$
P(X_j=x_i)=\frac{1}{N}.
$$

But the observations are not independent, because earlier draws remove possible values for later draws.

For distinct previous draws,

$$
P(X_j=x_i\mid X_1=x_{i_1},\ldots,X_{j-1}=x_{i_{j-1}})
=\frac{1}{N-j+1}
$$

only if $x_i$ has not already been selected, and is $0$ otherwise.

Thus sampling without replacement gives identically distributed observations, but not independent observations. When $N$ is large compared with $n$, the dependence is often weak enough that iid approximations become accurate.

Related: [[Random sample]], [[Sampling distribution]], [[Independence]].
