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
  - "Test3_page_001.png"
---

# Quiz problem - no UMP two-sided normal test

## Restatement

Let $X_1,\ldots,X_n$ be a random sample from $N(\theta,\sigma^2)$ with known $\sigma^2$. Show that there is no uniformly most powerful test for

$$
H_0:\theta=\theta_0
\qquad\text{versus}\qquad
H_A:\theta\ne\theta_0.
$$

## Solution

For a fixed alternative $\theta_1>\theta_0$, [[Neyman-Pearson lemma]] gives the most powerful level $\alpha$ test:

$$
\bar X>c_+.
$$

It rejects in the right tail.

For a fixed alternative $\theta_2<\theta_0$, the most powerful level $\alpha$ test is

$$
\bar X<c_-.
$$

It rejects in the left tail.

A single level $\alpha$ test cannot be both the right-tail most powerful test for every $\theta_1>\theta_0$ and the left-tail most powerful test for every $\theta_2<\theta_0$.

Therefore no [[UMP test]] exists for this two-sided normal alternative.

This is why two-sided normal tests are often derived as unbiased or likelihood-ratio tests, not as UMP tests.

## Links

- [[Neyman-Pearson lemma]]
- [[UMP test]]
- [[Most powerful test]]
- [[Unbiased test]]
- [[Normal mean simple LRT]]
