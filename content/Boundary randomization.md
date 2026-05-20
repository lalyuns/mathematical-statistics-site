---
created: 2026-05-21
aliases:
  - 邊界隨機化讓 likelihood ratio test 剛好用滿 size alpha
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - likelihood-ratio-tests
  - randomized-tests
  - proofs
source:
  - "[[Topic 5 revised]]"
---

# Boundary randomization

[[Boundary randomization]] makes an LR test hit exact size $\alpha$.

Let

$$C_0=\{x:L(\theta_A)>kL(\theta_0)\},\qquad C_1=\{x:L(\theta_A)=kL(\theta_0)\}.$$

If $P_{\theta_0}(C_0)=\alpha_\ell$ and $P_{\theta_0}(C_0\cup C_1)=\alpha_u$, reject on $C_1$ with probability

$$\gamma=\frac{\alpha-\alpha_\ell}{\alpha_u-\alpha_\ell}.$$

Then $E_{\theta_0}[\varphi(X)]=\alpha$.

Related: [[Randomized test]], [[Neyman-Pearson lemma]], [[Size and level]].