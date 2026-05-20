---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - asymptotics
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_006.png
  - Topic 4_revised_page_007.png
---

# Asymptotic normality of MLE

Under regularity conditions,

$$
\sqrt n(\hat\theta-\theta_0)\xrightarrow{d}
N(0,I(\theta_0)^{-1}).
$$

The MLE is consistent and asymptotically efficient in regular one-parameter models.

## Proof skeleton with missing steps

Let $\ell(\theta)=\sum_{i=1}^n\log f(X_i\mid\theta)$ and $S(\theta)=\partial_\theta\ell(\theta)$.

At an interior MLE,

$$
S(\hat\theta_n)=0.
$$

Taylor expand around the true value $\theta_0$:

$$
0=S(\hat\theta_n)
=S(\theta_0)+\partial_\theta S(\theta^*)(\hat\theta_n-\theta_0),
$$

where $\theta^*$ lies between $\hat\theta_n$ and $\theta_0$. Since $\partial_\theta S(\theta)=\partial_\theta^2\ell(\theta)$, write observed information as

$$
I_n(\theta^*)=-\partial_\theta^2\ell(\theta^*).
$$

Then

$$
\frac{1}{\sqrt n}S(\theta_0)
-\left(\frac1n I_n(\theta^*)\right)\sqrt n(\hat\theta_n-\theta_0)=0.
$$

By [[Central limit theorem]],

$$
\frac{1}{\sqrt n}S(\theta_0)\xrightarrow{d}N(0,I_0(\theta_0)).
$$

By [[Weak law of large numbers]] and [[Regularity conditions]],

$$
\frac1n I_n(\theta^*)\xrightarrow{p}I_0(\theta_0).
$$

Then [[Slutsky theorem]] gives

$$
\sqrt n(\hat\theta_n-\theta_0)
\xrightarrow{d}N(0,I_0(\theta_0)^{-1}).
$$

For a smooth function $\tau(\theta)$, the delta method gives

$$
\sqrt n(\tau(\hat\theta_n)-\tau(\theta_0))
\xrightarrow{d}
N(0,\tau'(\theta_0)^2 I_0(\theta_0)^{-1}).
$$

Related: [[Central limit theorem]], [[Score function]], [[Fisher information]], [[Regularity conditions]], [[Slutsky theorem]], [[Delta method]], [[Cramer-Rao lower bound]].
