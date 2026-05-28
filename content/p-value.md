---
created: 2026-05-20
aliases:
  - p-value 是觀察到的顯著水準
  - observed significance level
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

# p-value

A [[p-value]] is an observed significance level: a statistic between 0 and 1 where smaller values give stronger evidence against [[Null hypothesis]].

To be usable as a level rule, it must be a [[Valid p-value]].

For the two-sided normal mean test with unknown variance from [[Normal mean LRT with unknown variance]],

$$
T_n=\frac{\bar X_n-\mu_0}{S_n/\sqrt n},
$$

the lecture writes the p-value as

$$
p(x)=
\begin{cases}
2P\left(T_n>\dfrac{\bar x_n-\mu_0}{s_n/\sqrt n}\right)
=2\left[
1-\Phi_{n-1}\left(\dfrac{\bar x_n-\mu_0}{s_n/\sqrt n}\right)
\right],
& \bar x_n-\mu_0>0,\\[1.2em]
2P\left(T_n<\dfrac{\bar x_n-\mu_0}{s_n/\sqrt n}\right)
=2\Phi_{n-1}\left(\dfrac{\bar x_n-\mu_0}{s_n/\sqrt n}\right),
& \bar x_n-\mu_0<0,
\end{cases}
$$

where $\Phi_{n-1}$ is the cdf of the $t_{n-1}$ distribution.
