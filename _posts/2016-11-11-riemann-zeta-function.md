---
layout: post
title:  "Riemann Zeta Function"
date:   2016-11-11 09:11:03
description: Zeta. Pellent aliquet nibh nec urna. In nis aliquet vel, dapibus id,mattis.
thumbnail: my-cathedral-by-philippe-clairo-navajo-nation-parks-2560x1600.jpg
categories: [category1, crypto, math, number-theory]

# Information for the author block
author: Shift Shuffle
---

# Riemann Zeta Function

Bernhardt Rieman, 1826-1866

$$\zeta(s) = \displaystyle{\sum \frac{1}{n^s}} $$

$$\{s \in \mathbb{C} \, \mid \, Re(s) > 1 \}$$


# Euler Product
$$.$$

$$\zeta(s) = \displaystyle{\prod_{p} (1-p^{-s})^{-1}} $$

where the product is over all primes $$p$$


# The sum of reciprocal of primes diverges

If $$\, \vert x \vert < 1 \,$$ then $$\log (1-x) = - \displaystyle{\sum_{r=1}^{\infty} \frac{x^r}{r}}$$

$$\log \zeta(s) = \log \displaystyle{\prod_{p} (1-p^{-s})^{-1}}$$

$$= - \displaystyle{\sum_{p} \log \left( 1-\frac{1}{p^s} \right)} $$

$$=\displaystyle{\sum_{p}\sum_{r=1}^{\infty} \frac{1}{rp^{rs}}}$$

but $$ \, \lim_{s \to 1^{+}}\zeta(s) = \infty \,
$$ since harmonic series diverges,
it follows that $$ \, \lim_{s \to 1^{+}}\log \zeta(s) = \infty \,
$$ as well.

$$\displaystyle{\sum_{p}\sum_{r=1}^{\infty} \frac{1}{rp^{rs}}} = \displaystyle{\sum_{p} \frac{1}{p^{s}}} + \displaystyle{\sum_{p}\sum_{r=2}^{\infty} \frac{1}{rp^{rs}}} $$

But

$$\displaystyle{\sum_{p} \frac{1}{p^{s}}} + \displaystyle{\sum_{p}\sum_{r=2}^{\infty} \frac{1}{rp^{rs}}} <
\displaystyle{\sum_{p} \frac{1}{p^{s}}} + \displaystyle{\sum_{p}\sum_{r=2}^{\infty} \frac{1}{p^{r}}} $$


Furthermore $$\displaystyle{\sum_{r=2}^{\infty} \frac{1}{p^{r}}} = \frac{1}{p(p-1)}$$

Hence,

$$\displaystyle{\sum_{p}\sum_{r=2}^{\infty} \frac{1}{rp^{rs}}} <
\displaystyle{\sum_{p} \frac{1}{p(p-1)}} <
\displaystyle{\sum_{n} \frac{1}{n(n-1)}}
$$

which converges (limit comparison test). So

$$ \displaystyle \lim_{s \to 1^{+}} \sum_{p} \frac{1}{p^s} = \sum_{p} \frac{1}{p} $$

diverges $$\small \blacksquare$$





### Ut Labore et Dolore

Ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. Lorem ipsum dolor sit amet:

1. consectetur adipisicing elit
2. sed do eiusmod tempor incididunt
3. ut labore et dolore magna aliqua.

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

[link1]: example.net
[link2]: example.com
[link3]: example.org
