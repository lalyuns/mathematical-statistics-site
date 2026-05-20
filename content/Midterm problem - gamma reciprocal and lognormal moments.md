---
created: 2026-05-21
categories:
  - Problems
topics:
  - Probability
tags:
  - statistics
  - midterm
  - moments
source:
  - "[[Topic 2 revised]]"
pages:
  - Test2_1_page_001.png
aliases:
  - Reciprocal gamma and lognormal moments
---

# Midterm problem - gamma reciprocal and lognormal moments

## Restatement

1. If $X\sim \operatorname{Gamma}(\alpha,\lambda)$ with rate $\lambda$, find $E(1/X)$ and $\operatorname{Var}(1/X)$.
2. If $\log Y\sim N(\mu,\sigma^2)$, find $E(Y)$ and $\operatorname{Var}(Y)$.

## Solution

For $X\sim \operatorname{Gamma}(\alpha,\lambda)$,

$$
f(x)=\frac{\lambda^\alpha}{\Gamma(\alpha)}x^{\alpha-1}e^{-\lambda x},\qquad x>0.
$$

For $k<\alpha$,

$$
E(X^{-k})=\frac{\lambda^k\Gamma(\alpha-k)}{\Gamma(\alpha)}.
$$

So, for $\alpha>1$,

$$
E(1/X)=\frac{\lambda}{\alpha-1}.
$$

For $\alpha>2$,

$$
E(1/X^2)=\frac{\lambda^2}{(\alpha-1)(\alpha-2)}.
$$

Therefore

$$
\operatorname{Var}(1/X)
=\frac{\lambda^2}{(\alpha-1)(\alpha-2)}
-\frac{\lambda^2}{(\alpha-1)^2}
=\frac{\lambda^2}{(\alpha-1)^2(\alpha-2)}.
$$

If $\log Y\sim N(\mu,\sigma^2)$, then $Y=e^Z$ with $Z\sim N(\mu,\sigma^2)$. Using the normal MGF,

$$
E(Y)=E(e^Z)=\exp\left(\mu+\frac{\sigma^2}{2}\right),
$$

and

$$
E(Y^2)=E(e^{2Z})=\exp(2\mu+2\sigma^2).
$$

Thus

$$
\operatorname{Var}(Y)
=\exp(2\mu+\sigma^2)\left(e^{\sigma^2}-1\right).
$$

## Linked knowledge

- [[Expectation]]
- [[Moment generating function]]
- [[Common distributions]]

