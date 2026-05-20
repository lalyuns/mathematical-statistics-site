---
created: 2026-05-20
aliases:
  - 常態平均數的簡單假設 LRT 會化成樣本平均數的單尾檢定
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - normal-tests
  - likelihood-ratio-tests
source:
  - "[[Topic 5 revised]]"
pages:
  - "page_004.png"
---

# Normal mean simple LRT

For $X_i\overset{iid}{\sim}N(\mu,\sigma^2)$ with known $\sigma^2$, test

$$H_0:\mu=\mu_0,\qquad H_A:\mu=\mu_1.$$

The [[Likelihood ratio test]] depends only on $\bar X_n$. If $\mu_1<\mu_0$, reject for small $\bar X_n$; if $\mu_1>\mu_0$, reject for large $\bar X_n$.

The [[Critical value]] is chosen under $H_0$, where

$$\bar X_n\sim N\left(\mu_0,\frac{\sigma^2}{n}\right).$$

By [[Neyman-Pearson lemma]], this is the MP size $\alpha$ test.