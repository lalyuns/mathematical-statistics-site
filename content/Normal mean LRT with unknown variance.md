---
created: 2026-05-20
aliases:
  - 未知變異數的常態平均數 LRT 會化成 t 檢定
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
  - "page_005.png"
---

# Normal mean LRT with unknown variance

For $X_i\overset{iid}{\sim}N(\mu,\sigma^2)$ with unknown $\sigma^2$, test

$$H_0:\mu=\mu_0,\qquad H_A:\mu\ne\mu_0.$$

The [[Likelihood ratio test]] reduces to rejecting large

$$\left|\frac{\bar X_n-\mu_0}{S_n/\sqrt n}\right|.$$

In the lecture notation,

$$
\Theta_0=\{(\mu_0,\sigma^2):\sigma^2>0\},
\qquad
\Theta=\{(\mu,\sigma^2):-\infty<\mu<\infty,\sigma^2>0\}.
$$

So $\dim(\Theta)-\dim(\Theta_0)=2-1=1$.

The restricted and unrestricted variance MLEs are

$$
\hat\sigma_0^2=\frac1n\sum_{i=1}^n(X_i-\mu_0)^2,
\qquad
\hat\sigma_n^2=\frac1n\sum_{i=1}^n(X_i-\bar X_n)^2.
$$

The LRT rejects for small

$$
\lambda(X_1,\ldots,X_n)
=\left(\frac{\hat\sigma_n^2}{\hat\sigma_0^2}\right)^{-n/2},
$$

which is equivalent to rejecting for large

$$
\frac{(\bar X_n-\mu_0)^2}{\hat\sigma_n^2}.
$$

With

$$
S_n=\sqrt{\frac{n}{n-1}\hat\sigma_n^2},
\qquad
T_n=\frac{\bar X_n-\mu_0}{S_n/\sqrt n},
$$

the exact size $\alpha$ LRT has test function

$$
\varphi(T_n)=1_{\{|T_n|>t_{n-1,1-\alpha/2}\}}.
$$

A separate [[Asymptotic test]] uses

$$
-2\log\lambda(X_1,\ldots,X_n)
=n(\log\hat\sigma_n^2-\log\hat\sigma_0^2)
\xrightarrow{d}\chi^2_1
$$

under $H_0$.

Related: [[t confidence interval]], [[Test inversion]].
