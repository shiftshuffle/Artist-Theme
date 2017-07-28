---
layout: post
title:  "I Make Music Too"
date:   2010-11-11 09:11:03
description: Phasellus hendrerit. Pellent aliquet nibh nec urna. In nis aliquet vel, dapibus id,mattis.
thumbnail: food2.jpg
categories: [category1,math,analytic,combinatoric]

# Information for the author block
author: Shift Shuffle
---

Bernoulli numbers are defined as de coefficients  $B(n) $ when expanding

$$   \frac{ x }{  e^{x} - 1 } = \displaystyle{\sum_{n=0}^{\infty}  B_{n} \frac{  x^{n}  }{ n! }}  $$

we have the following relation:

$$ - e^{x} + x +1 =  \displaystyle{  \left(\! \sum_{n=1}^{\infty} B_{n} \frac{  x^{n}  }{ n! }    \!\right)   \left(\!  \sum_{k=1}^{\infty}  \frac{  x^{k}  }{ k! }   \!\right)}   $$



$$   \ \    $$
$$   \ \    $$

$$ \Longrightarrow   $$

$$   \ \    $$
$$   \ \    $$


$$ -   \sum_{j=2}^{\infty}  \frac{  x^{j}  }{ j! }  =  \sum_{k=2}^{\infty}  \frac{  x^{k} }{ k! }  \sum_{l=1}^{k-1}  \left(\!  \begin{array}{c}  k \\  l  \end{array}  \!\right)  B_{l} \qquad (1)$$






$$   \ \    $$
$$   \ \    $$

Remember Cauchy Convolution :

$$   \displaystyle{  \left(\! \sum_{i=0}^{\infty} a_{i}  x^{i}     \!\right)   \left(\! \sum_{j=0}^{\infty}  b_{j}  x^{j}    \!\right) =  \sum_{k=0}^{\infty} c_{k}  x^{k}}  $$


Where

$$   c_{k} = \sum_{l=0}^{k} a_{l}  b_{k-l}   $$

$$   \ \    $$
$$   \ \    $$


if we apply it here  $$  \displaystyle{  \left(\! \sum_{n=1}^{\infty} B_{n} \frac{  x^{n} }{ n! }    \!\right)   \left(\!  \sum_{k=1}^{\infty}  \frac{  x^{k}  }{ k! }   \!\right) = \sum_{k=2}^{\infty} c_{k}  x^{k}} $$

and


$$   c_{k} = \sum_{l=1}^{k-1}\begin{eqnarray} \frac{ B_{l} }{ l! ( k - l )! } \end{eqnarray}  =  \frac{  1  }{ k! }  \sum_{l=1}^{k-1}  \left(\! \begin{array}{c} k \\ l  \end{array} \!\right)  B_{l} $$

$$   \ \    $$
$$   \ \    $$

now that we have derived $\qquad (1)$  we equate coefficients and get
$$  \sum_{l=1}^{k-1}  \left(\!  \begin{array}{c}  k \\  l  \end{array}  \!\right)  B_{l} = -1  $$

$$   \ \    $$
$$   \ \    $$

$$  \sum_{l=1}^{k-1}  \left(\!  \begin{array}{c}    k \\ l  \end{array}  \!\right)  B_{l} = - \left(\!  \begin{array}{c}  k \\  0  \end{array}  \!\right) B_{0}$$

taking in account $ B_{0}=1    $

We get
$$   \ \    $$
$$   \ \    $$

$$   \begin{eqnarray} \sum_{l=1}^{k-1}  \left(\!  \begin{array}{c}  k \\  l  \end{array}   \!\right)  B_{l} = \begin{cases} 1& ,  k= 1  \\ 0 & ,  k \geqq 2 \end{cases} \end{eqnarray} $$


Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut [enim ad minim][link1] veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Let's test some inline math $x$, $y$, $x_1$, $y_1$.

Now a inline math with special character: $|\psi\rangle$, $x'$, $x^\*$.

Test a display math:
$$
   |\psi_1\rangle = a|0\rangle + b|1\rangle
$$
Is it O.K.?

Test a display math with equation number:
\begin{equation}
   |\psi_1\rangle = a|0\rangle + b|1\rangle
\end{equation}
Is it O.K.?

Test a display math with equation number:
$$
  \begin{align}
    |\psi_1\rangle &= a|0\rangle + b|1\rangle \\\\
    |\psi_2\rangle &= c|0\rangle + d|1\rangle
  \end{align}
$$
Is it O.K.?







###Ut Labore et Dolore

Ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. Lorem ipsum dolor sit amet:

1. consectetur adipisicing elit
2. sed do eiusmod tempor incididunt
3. ut labore et dolore magna aliqua.

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

[link1]: example.net
[link2]: example.com
[link3]: example.org
