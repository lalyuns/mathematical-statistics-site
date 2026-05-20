---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Point estimation]]"
tags:
  - statistics
  - likelihood
  - estimation
source:
  - "[[Topic 4 revised]]"
pages:
  - Topic 4_revised_page_002.png
  - Topic 4_revised_page_003.png
  - Topic 4_revised_page_007.png
---

# Fisher information

For one observation, the Fisher information is

$$
I_0(\theta)=\operatorname{Var}_\theta(\partial_\theta\log f(X\mid\theta)).
$$

Because the [[Score function]] has mean zero under regularity conditions,

$$
I_0(\theta)=E_\theta[(\partial_\theta\log f(X\mid\theta))^2].
$$

If second derivatives can be interchanged with integration, then

$$
I_0(\theta)=-E_\theta[\partial_\theta^2\log f(X\mid\theta)].
$$

For iid data, the sample information is additive:

$$
I_n(\theta)=nI_0(\theta).
$$

This additivity is why the one-parameter [[Cramer-Rao lower bound]] has denominator $nI_0(\theta)$.

Related: [[Score function]], [[Regularity conditions]], [[Asymptotic normality of MLE]].
