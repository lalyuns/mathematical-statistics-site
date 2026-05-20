---
created: 2026-05-21
categories:
  - Problems
topics:
  - Joint distributions
tags:
  - statistics
  - midterm
  - transformations
source:
  - "[[Topic 2 revised]]"
pages:
  - Test2_2_page_001.png
aliases:
  - Spherical coordinates for three standard normals
---

# Midterm problem - spherical normal transformation

## Restatement

Let $X,Y,Z$ be independent standard normal random variables. Use spherical coordinates

$$
X=R\sin\Phi\cos\Theta,\quad
Y=R\sin\Phi\sin\Theta,\quad
Z=R\cos\Phi
$$

to find the joint density of $(R,\Theta,\Phi)$.

## Solution

The joint density of $(X,Y,Z)$ is

$$
(2\pi)^{-3/2}\exp\left(-\frac{x^2+y^2+z^2}{2}\right).
$$

Under the spherical transformation,

$$
x^2+y^2+z^2=r^2,
$$

and the Jacobian is

$$
r^2\sin\phi.
$$

Therefore

$$
f_{R,\Theta,\Phi}(r,\theta,\phi)
=(2\pi)^{-3/2}e^{-r^2/2}r^2\sin\phi,
$$

for

$$
r>0,\qquad 0<\theta<2\pi,\qquad 0<\phi<\pi.
$$

The factorization shows that $\Theta$ is uniform on $(0,2\pi)$, $R$ has the chi distribution with $3$ degrees of freedom, and the angular density for $\Phi$ is proportional to $\sin\phi$.

## Linked knowledge

- [[Spherical transformation]]
- [[Transformation of random variables]]
- [[Joint distribution]]
- [[Common distributions]]

