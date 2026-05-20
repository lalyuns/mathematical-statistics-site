---
created: 2026-05-21
aliases:
  - Likelihood ratio rejection region 讓檢定函數差與密度差同號
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - likelihood-ratio-tests
  - proofs
source:
  - "[[Topic 5 revised]]"
---

# LR rejection region sign argument

[[Neyman-Pearson lemma]] rests on the pointwise inequality

$$(\varphi(x)-\psi(x))(f_A(x)-kf_0(x))\ge 0.$$

The LR [[Rejection region]] is where $f_A(x)>kf_0(x)$. There, $\varphi(x)=1$ and $\varphi(x)-\psi(x)\ge0$.

Outside the rejection region, $f_A(x)<kf_0(x)$ and $\varphi(x)=0$, so $\varphi(x)-\psi(x)\le0$.

On the boundary, the density difference is zero. The product is nonnegative everywhere.

Related: [[Boundary randomization]], [[Most powerful test]].