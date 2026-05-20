---
created: 2026-05-21
categories:
  - "[[Evergreen]]"
topics:
  - "[[Likelihood ratio tests]]"
tags:
  - statistics
  - quizzes
  - likelihood-ratio-tests
source:
  - "[[Quiz 2 hypothesis testing problems MOC]]"
pages:
  - "Test2_page_001.png"
  - "Test3_page_001.png"
---

# Quiz problem - binomial equal proportions LRT

## Restatement

Suppose $X_1,\ldots,X_m$ are independent with

$$
X_i\sim\operatorname{Binomial}(n,p_i).
$$

Derive a likelihood ratio test for

$$
H_0:p_1=\cdots=p_m
$$

versus the alternative that $p_i\ne p_j$ for some $i\ne j$. Find the large-sample distribution of the test statistic.

## Solution

Let

$$
x_+=\sum_{i=1}^m x_i,\qquad \hat p=\frac{x_+}{mn},\qquad \hat p_i=\frac{x_i}{n}.
$$

Under the unrestricted model, the MLE is $\hat p_i=x_i/n$ for each group.

Under $H_0$, the common-proportion MLE is

$$
\hat p=\frac{x_+}{mn}.
$$

Ignoring binomial coefficients that cancel in the likelihood ratio,

$$
\lambda(x)
=
\frac{\hat p^{x_+}(1-\hat p)^{mn-x_+}}
{\prod_{i=1}^m \hat p_i^{x_i}(1-\hat p_i)^{n-x_i}}.
$$

The LRT rejects for small $\lambda(x)$, equivalently for large

$$
G^2=-2\log\lambda(x).
$$

Expanding,

$$
G^2
=
2\sum_{i=1}^m
\left[
x_i\log\left(\frac{\hat p_i}{\hat p}\right)
+(n-x_i)\log\left(\frac{1-\hat p_i}{1-\hat p}\right)
\right].
$$

The full model has dimension $m$. The null model has dimension $1$. By [[Wilks theorem]],

$$
G^2\xrightarrow{d}\chi^2_{m-1}
$$

under $H_0$.

## Links

- [[Likelihood ratio test]]
- [[Likelihood ratio statistic]]
- [[Wilks theorem]]
- [[Asymptotic test]]
