---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Convergence]]"
tags:
  - statistics
  - convergence
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_005.png
  - Topic 3_revised_page_006.png
---

# Weak law of large numbers

The [[Weak law of large numbers]] says that for iid $X_i$ with mean $\mu$,

$$
\bar X_n\xrightarrow{p}\mu.
$$

It is often proved with Chebyshev's inequality when the variance is finite:

$$
P(|\bar X_n-\mu|>\epsilon)
\le \frac{\operatorname{Var}(\bar X_n)}{\epsilon^2}
=\frac{\sigma^2}{n\epsilon^2}\to0.
$$

Related: [[Strong law of large numbers]], [[Convergence in probability]], [[Sample mean and sample variance]].
