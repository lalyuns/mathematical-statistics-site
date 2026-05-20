---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
tags:
  - statistics
  - quizzes
  - hypothesis-tests
source:
  - "[[Quiz 2 hypothesis testing problems MOC]]"
pages:
  - "Test2_page_001.png"
  - "Test3_page_001.png"
---

# Quiz problem - UMP tests are unbiased

## Restatement

Show that a uniformly most powerful level $\alpha$ test is unbiased.

The quiz wording says "(1 - alpha) uniformly most powerful test" in some versions, but the content matches the standard result: a [[UMP test]] of [[Level alpha test|level alpha]] is an [[Unbiased test]].

## Solution

Let $\varphi$ be a UMP level $\alpha$ test with [[Power function]] $\beta_\varphi(\theta)$.

Compare it with the randomized test $\psi$ that rejects with constant probability $\alpha$:

$$
\psi(x)=\alpha.
$$

Its power is constant:

$$
\beta_\psi(\theta)=\alpha
$$

for every $\theta$.

Since $\varphi$ is UMP among level $\alpha$ tests,

$$
\beta_\varphi(\theta_A)\ge \beta_\psi(\theta_A)=\alpha
$$

for all $\theta_A\in\Theta_A$.

Since $\varphi$ is level $\alpha$,

$$
\beta_\varphi(\theta_0)\le \alpha
$$

for all $\theta_0\in\Theta_0$.

Therefore

$$
\beta_\varphi(\theta_A)\ge\alpha\ge\beta_\varphi(\theta_0),
$$

so $\varphi$ is unbiased.

## Links

- [[UMP tests are unbiased]]
- [[Unbiased test]]
- [[Power function]]
- [[Level alpha test]]
