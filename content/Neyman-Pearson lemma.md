---
created: 2026-05-20
aliases:
  - NP lemma
  - Neyman-Pearson 引理
  - 簡單假設下的最強力檢定
  - Neyman-Pearson lemma 給出簡單假設下的最強力檢定
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_003.png"
  - "page_004.png"
---

# Neyman-Pearson lemma

For simple hypotheses

$$H_0:\theta=\theta_0,\qquad H_A:\theta=\theta_A,$$

[[Neyman-Pearson lemma]] says that the LR test is [[Most powerful test]] among all [[Level alpha test|level alpha tests]].

The test rejects where $L(\theta_A)>kL(\theta_0)$, randomizing on the boundary if needed.

In the lecture notation, define

$$
C_0=\{x:L(\theta_A)>kL(\theta_0)\},
\qquad
C_1=\{x:L(\theta_A)=kL(\theta_0)\}.
$$

Let

$$
P_{\theta_0}(X\in C_0)=\alpha_\ell\le\alpha,
\qquad
P_{\theta_0}(X\in C_0\cup C_1)=\alpha_u\ge\alpha.
$$

Then the size $\alpha$ LR test has test function

$$
\varphi(X)=I_{C_0}(X)+
\frac{\alpha-\alpha_\ell}{\alpha_u-\alpha_\ell}I_{C_1}(X).
$$

Its null rejection probability is

$$
E_{\theta_0}[\varphi(X)]
=\alpha_\ell+
\frac{\alpha-\alpha_\ell}{\alpha_u-\alpha_\ell}(\alpha_u-\alpha_\ell)
=\alpha.
$$

## Proof

Let $\varphi$ be the LR test and $\psi$ any other level $\alpha$ test. We need

$$E_{\theta_A}[\varphi(X)]\ge E_{\theta_A}[\psi(X)].$$

By [[LR rejection region sign argument]],

$$(\varphi(x)-\psi(x))(f_A(x)-kf_0(x))\ge0.$$

Integrating and expanding gives

$$\int(\varphi-\psi)f_A\,dx\ge k\int(\varphi-\psi)f_0\,dx.$$

Using [[Power function]], this is

$$\beta_\varphi(\theta_A)-\beta_\psi(\theta_A)\ge k(\beta_\varphi(\theta_0)-\beta_\psi(\theta_0)).$$

By [[Boundary randomization]], $\beta_\varphi(\theta_0)=\alpha$. Since $\psi$ is a [[Level alpha test]], $\beta_\psi(\theta_0)\le\alpha$. Therefore

$$\beta_\varphi(\theta_A)-\beta_\psi(\theta_A)\ge k(\alpha-\beta_\psi(\theta_0))\ge0.$$

So the LR test is most powerful.

## Proof ingredients

- [[Most powerful test]]
- [[LR rejection region sign argument]]
- [[Boundary randomization]]
- [[Level alpha test]]
- [[Power function]]
