---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Convergence]]"
tags:
  - statistics
  - asymptotics
source:
  - "[[Topic 3 revised]]"
pages:
  - Topic 3_revised_page_006.png
aliases:
  - CLT
  - Central Limit Theorem
  - 中央極限定理
---

# Central limit theorem

For iid $X_i$ with mean $\mu$ and variance $\sigma^2<\infty$,

$$
\frac{\sqrt n(\bar X_n-\mu)}{\sigma}\xrightarrow{d}N(0,1).
$$

[[Central limit theorem]] turns averages into approximate normal statistics.

Equivalently, for large $n$,

$$
\bar X_n\approx N\left(\mu,\frac{\sigma^2}{n}\right).
$$

## Proof by MGF, as in Topic 3

Let

$$
Z_i=\frac{X_i-\mu}{\sigma},
$$

so that $E[Z_i]=0$ and $\operatorname{Var}(Z_i)=1$. The standardized sample mean is

$$
Y_n=\frac{\sqrt n(\bar X_n-\mu)}{\sigma}
=\frac{1}{\sqrt n}\sum_{i=1}^n Z_i.
$$

By independence, the moment generating function of $Y_n$ factors:

$$
\begin{aligned}
M_{Y_n}(t)
&=E\left[\exp\left(t\frac{1}{\sqrt n}\sum_{i=1}^n Z_i\right)\right]\\
&=\prod_{i=1}^n E\left[e^{tZ_i/\sqrt n}\right]\\
&=\left(M_Z\left(\frac{t}{\sqrt n}\right)\right)^n.
\end{aligned}
$$

Using the second-order Taylor expansion of $M_Z(u)$ at $0$,

$$
M_Z(u)=1+uE[Z]+\frac{u^2}{2}E[Z^2]+o(u^2)
=1+\frac{u^2}{2}+o(u^2).
$$

With $u=t/\sqrt n$,

$$
M_Z\left(\frac{t}{\sqrt n}\right)
=1+\frac{t^2}{2n}+o\left(\frac1n\right).
$$

Therefore

$$
M_{Y_n}(t)
=\left(1+\frac{t^2}{2n}+o\left(\frac1n\right)\right)^n
\to e^{t^2/2}.
$$

The limit $e^{t^2/2}$ is the MGF of $N(0,1)$. By [[MGF continuity theorem]],

$$
Y_n\xrightarrow{d}N(0,1).
$$

Important caveat: this MGF proof assumes the MGF exists in a neighborhood of $0$. The full iid finite-variance CLT is more general and is usually proved using characteristic functions.

## How to use it

When a probability involves $\bar X_n$, standardize first:

$$
P(|\bar X_n-\mu|<c)
=P\left(-\frac{\sqrt n c}{\sigma}
<\frac{\sqrt n(\bar X_n-\mu)}{\sigma}
<\frac{\sqrt n c}{\sigma}\right)
\approx 2\Phi\left(\frac{\sqrt n c}{\sigma}\right)-1.
$$

Related: [[Convergence in distribution]], [[Moment generating function]], [[MGF continuity theorem]], [[Asymptotic test]], [[Delta method]].
