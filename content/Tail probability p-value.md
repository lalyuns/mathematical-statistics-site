---
created: 2026-05-20
aliases:
  - 尾端機率構造會產生 valid p-value
categories:
  - "[[Evergreen]]"
topics:
  - "[[Hypothesis testing]]"
tags:
  - statistics
  - p-values
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_007.png"
---

# Tail probability p-value

If large $W(X)$ supports [[Alternative hypothesis]], define

$$p(x)=\sup_{\theta\in\Theta_0}P_\theta(W(X)\ge W(x)).$$

This is a [[Valid p-value]]. It asks how extreme the observed statistic is under the null, using the worst-case null parameter.

## Why it is valid

For fixed $\theta\in\Theta_0$, define

$$
p_\theta(x)=P_\theta(W(X)\ge W(x)).
$$

By the probability integral transform applied to the null distribution of the tail statistic,

$$
P_\theta(p_\theta(X)\le \alpha)\le \alpha.
$$

The supremum p-value satisfies $p(x)=\sup_{\theta\in\Theta_0}p_\theta(x)\ge p_\theta(x)$, so

$$
\{p(X)\le\alpha\}\subseteq \{p_\theta(X)\le\alpha\}.
$$

Therefore

$$
P_\theta(p(X)\le\alpha)\le\alpha
$$

for every null $\theta$, proving validity.

Related: [[p-value]], [[Valid p-value]], [[Observed significance level]], [[Level alpha test]].
