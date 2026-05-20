---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Confidence set]]"
tags:
  - statistics
  - confidence-sets
  - hypothesis-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - page_008.png
aliases:
  - Test inversion duality
---

# Test confidence duality

[[Test confidence duality]] says that a family of level $\alpha$ tests and a confidence set are two views of the same object.

If $A(\theta_0)$ is the acceptance region of a level $\alpha$ test for $H_0:\theta=\theta_0$, define

$$
C(x)=\{\theta_0:x\in A(\theta_0)\}.
$$

Then

$$
P_\theta(\theta\in C(X))
=P_\theta(X\in A(\theta))
\ge 1-\alpha.
$$

So $C(X)$ is a $(1-\alpha)$ confidence set.

Conversely, if $C(X)$ has coverage at least $1-\alpha$, then for testing $H_0:\theta=\theta_0$, use

$$
A(\theta_0)=\{x:\theta_0\in C(x)\}.
$$

Then

$$
P_{\theta_0}(X\notin A(\theta_0))
=P_{\theta_0}(\theta_0\notin C(X))
\le \alpha,
$$

so the induced test has level $\alpha$.

Related: [[Test inversion]], [[Confidence set]], [[Acceptance region]], [[Level alpha test]].
