---
created: 2026-05-20
aliases:
  - 常態平均數的簡單假設 LRT 會化成樣本平均數的單尾檢定
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - normal-tests
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_004.png"
---

# Normal mean simple LRT

For $X_i\overset{iid}{\sim}N(\mu,\sigma^2)$ with known $\sigma^2$, test

$$H_0:\mu=\mu_0,\qquad H_A:\mu=\mu_1.$$

The [[Likelihood ratio test]] depends only on $\bar X_n$. If $\mu_1<\mu_0$, reject for small $\bar X_n$; if $\mu_1>\mu_0$, reject for large $\bar X_n$.

The likelihood-ratio statistic is

$$
\lambda(X_1,\ldots,X_n)
=
\frac{
\exp\left(-\sum_{i=1}^n(X_i-\mu_0)^2/(2\sigma^2)\right)
}{
\exp\left(-\sum_{i=1}^n(X_i-\mu_1)^2/(2\sigma^2)\right)
}
=
\exp\left(
\frac{-2n\bar X_n(\mu_1-\mu_0)-n\mu_0^2+n\mu_1^2}{2\sigma^2}
\right).
$$

Therefore $\lambda(X)<\lambda^*$ is equivalent to

$$
\bar X_n<c_1\quad\text{if }\mu_1-\mu_0<0,
\qquad
\bar X_n>c_2\quad\text{if }\mu_1-\mu_0>0.
$$

The [[Critical value]] is chosen under $H_0$, where

$$\bar X_n\sim N\left(\mu_0,\frac{\sigma^2}{n}\right).$$

Thus, for a size $\alpha$ test,

$$
\frac{c_1-\mu_0}{\sigma/\sqrt n}=z_\alpha,
\qquad
\frac{c_2-\mu_0}{\sigma/\sqrt n}=z_{1-\alpha},
$$

so

$$
c_1=\mu_0+z_\alpha\frac{\sigma}{\sqrt n},
\qquad
c_2=\mu_0-z_\alpha\frac{\sigma}{\sqrt n}.
$$

By [[Neyman-Pearson lemma]], this is the MP size $\alpha$ test.
