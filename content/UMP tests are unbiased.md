---
created: 2026-05-20
aliases:
  - UMP level alpha test 會是無偏檢定
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
tags:
  - statistics
  - hypothesis-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_002.png"
---

# UMP tests are unbiased

A UMP level $\alpha$ test is an [[Unbiased test]].

Compare it with the randomized test that rejects with constant probability $\alpha$. UMP implies $\beta(\theta_A)\ge\alpha$ on the alternative. Level $\alpha$ implies $\beta(\theta_0)\le\alpha$ on the null.

Thus $\beta(\theta_A)\ge\beta(\theta_0)$.

## Proof with the skipped comparison test

Let $\varphi$ be the UMP level $\alpha$ test. Compare it with the randomized test

$$
\varphi^*(x)=\alpha.
$$

This competitor has constant power

$$
\beta^*(\theta)=E_\theta[\varphi^*(X)]=\alpha.
$$

Since $\varphi$ is UMP among level $\alpha$ tests,

$$
\beta_\varphi(\theta_A)\ge \beta^*(\theta_A)=\alpha
$$

for every $\theta_A\in\Theta_A$. Since $\varphi$ is level $\alpha$,

$$
\beta_\varphi(\theta_0)\le\alpha
$$

for every $\theta_0\in\Theta_0$. Hence

$$
\beta_\varphi(\theta_A)\ge \beta_\varphi(\theta_0),
$$

which is the definition of an unbiased test.

Related: [[UMP test]], [[Level alpha test]], [[Power function]], [[Randomized test]].
