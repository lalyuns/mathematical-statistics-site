---
created: 2026-05-20
aliases:
  - Valid p-value 控制虛無假設下小 p-value 的機率
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
  - "page_006.png"
---

# Valid p-value

A [[Valid p-value]] satisfies

$$\sup_{\theta\in\Theta_0}P_\theta(p(X)\le\alpha)\le\alpha$$

for every $0\le\alpha\le1$.

Then the rule $p(X)\le\alpha$ is a [[Level alpha test]].

The definition is exactly the type-I-error control condition for the test that rejects when $p(X)\le\alpha$.

Related: [[Tail probability p-value]], [[Observed significance level]].
