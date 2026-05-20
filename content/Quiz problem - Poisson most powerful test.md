---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - quizzes
  - likelihood-ratio-tests
source:
  - "[[Quiz 2 hypothesis testing problems MOC]]"
pages:
  - "Test2_page_001.png"
  - "Test3_page_001.png"
---

# Quiz problem - Poisson most powerful test

## Restatement

Let $X_1,\ldots,X_n$ be a random sample from $\operatorname{Poisson}(\lambda)$. Find the most powerful level $\alpha$ test for

$$
H_0:\lambda=\lambda_0
\qquad\text{versus}\qquad
H_A:\lambda=\lambda_1,\quad \lambda_1>\lambda_0.
$$

## Solution

Let

$$
S=\sum_{i=1}^n X_i.
$$

The likelihood is

$$
L(\lambda)\propto e^{-n\lambda}\lambda^S.
$$

The likelihood ratio in favor of $\lambda_1$ over $\lambda_0$ is

$$
\frac{L(\lambda_1)}{L(\lambda_0)}
=
e^{-n(\lambda_1-\lambda_0)}
\left(\frac{\lambda_1}{\lambda_0}\right)^S.
$$

Since $\lambda_1>\lambda_0$, this ratio is increasing in $S$.

By [[Neyman-Pearson lemma]], the most powerful level $\alpha$ test rejects for large $S$:

$$
\varphi(X)=1(S>c)+\gamma 1(S=c).
$$

Under $H_0$,

$$
S\sim\operatorname{Poisson}(n\lambda_0).
$$

Choose $c$ and $\gamma$ so that

$$
P_{\lambda_0}(S>c)+\gamma P_{\lambda_0}(S=c)=\alpha.
$$

Equivalently,

$$
\gamma=
\frac{\alpha-P_{\lambda_0}(S>c)}{P_{\lambda_0}(S=c)}
$$

for a cutoff $c$ satisfying

$$
P_{\lambda_0}(S>c)\le\alpha\le P_{\lambda_0}(S\ge c).
$$

## Links

- [[Neyman-Pearson lemma]]
- [[Most powerful test]]
- [[Boundary randomization]]
- [[Critical value]]
