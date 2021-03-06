---
layout: post
title: "Test math"
date: 2017-03-06
use_math: true
---

<p> This page illustrates "Mathjax" which can integrate mathematics into web pages.
Below is some miscellaneous mathematics. Note that the mathematics scales.. This is a web page, not a pdf file, it  automatically changes adjusts the width of the page if you change the width of the web page. One can also set a zoom feature on the mathematics. To see this 
point at a math formula and hold down the control key (on a Mac) and adjust the settings.
</p>
<p>
When $a \ne 0$ there are two solutions to \(ax^2 + bx + c = 0\) and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$  
\begin{equation*}
\psi=1-\phi=-\frac{1}{\phi}=\frac{1-\sqrt{5}}{2}=-0.61803989\ldots.
\end{equation*}
$$ A\Big( \begin{matrix}
      i & j & k\\
     t &u  &v\\
   \end{matrix}\Big),
   $$
</p>
<p>
<em>Theorem 1. </em>
Let $\Delta_A(\lambda)$  be the characteristic polynomial of the matrix $A$, that is 
\begin{equation}
\Delta_A(\lambda)=\det(\lambda I-A),
\end{equation}
 then 
\begin{equation}
\Delta_A(\lambda)=\sum_{k=0}^n (-1)^{n-k}\lambda^k \sigma_{n-k}(A)=
\sum_{k=0}^n (-1)^{k}\lambda^{n-k }\sigma_{k}(A). \label{eq:characteristic}
\end{equation}
where $\sigma_k(A)= $ the sum of all the principal minors of order $k$ of
$A$, with $\sigma_0(A)=1$.
</p>
<p>
<em>proof </em>
\begin{eqnarray*}
\Delta(\lambda )&=&\det[\lambda I-A]\\
&=&\sum_{k=0}^n(-1)^{n-k}\lambda^k\det[A : I]_{T_k}\\
&=&\sum_{k=0}^n(-1)^{n-k}\lambda ^k\sigma_{n-k}(A),
\end{eqnarray*}



\begin{align}
&\begin{bmatrix}
1&2&1\\2&4&2\\1&2&1
\end{bmatrix}
\begin{bmatrix}
x_1\\x_2\\x_3
\end{bmatrix}\\
&=(x_1+2x_2+x_3)\begin{bmatrix}
1\\2\\1\end{bmatrix}.\nonumber
\end{align}
$$\int_0^\infty e^{-x^2} dx $$

\begin{equation}
[a, b, c]=\left|
\begin{array}{ccc}
  a_1& a_2  & a_3  \\
 b_1 &b_2   & b_3  \\
 c_1 &c_2   &c_3   
\end{array}
\right|
\end{equation}
</p>

When $a \ne 0$, there are two solutions to \\(a~x^2 + b~x + c = 0\\) and they are
$$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

Let's test some inline math $x$, $y$, $x_1$, $y_1$. Now inline math with special character: $|\psi\rangle$, $x'$, $x^*$.

Test a display math:
$$
   |\psi_1\rangle = a|0\rangle + b|1\rangle
$$


Test a display math without equation number:
\begin{equation\*}
   |\psi_1\rangle = a|0\rangle + b|1\rangle
\end{equation\*}


Test a display math with equation number:
$$
  \begin{align}
    |\psi_1\rangle &= a|0\rangle + b|1\rangle \\
    |\psi_2\rangle &= c|0\rangle + d|1\rangle
  \end{align}
$$


And test a display math without equaltion number:
  \begin{align}
    |\psi_1\rangle &= a|0\rangle + b|1\rangle \\
    |\psi_2\rangle &= c|0\rangle + d|1\rangle
  \end{align}


Test a display math with equation number:
\begin{align}
    |\psi_1\rangle &= a|0\rangle + b|1\rangle \\\\
    |\psi_2\rangle &= c|0\rangle + d|1\rangle
\end{align}


And test a display math without equaltion number:
\begin{align\*}
    |\psi_1\rangle &= a|0\rangle + b|1\rangle \\\\
    |\psi_2\rangle &= c|0\rangle + d|1\rangle
\end{align\*}



# Module 2 : Modeling Discrete Time Systems by Pulse Transfer Function

## Lecture 1 : Motivation for using Z-transform


### 1. Motivation for using Z- Transform

In general, control system design methods can be classified as:

  * conventional or classical control techniques
  * modern control techniques

**Classical methods** use transform techniques and are based on transfer function models, whereas **modern techniques** are based on modeling of system by state variable methods.

Laplace transform is the basic tool of the classical methods in continuous domain. In principle, it can also be used for modeling digital control systems. However typical Laplace transform expressions of systems with digital or sampled signals contain exponential terms in the form of eTs which makes the manipulation in the Laplace domain difficult. This can be regarded as a motivation of using Z-transform.

Let the output of an ideal sampler be denoted by $f^*(t)$:
$$
  \begin{align}
    L[f^*(t)]	&=  F^*(s) \\
    &=  \sum_{k=0}^{\infty}f(kT)e^{-kTs}
  \end{align}
$$

Since $F^*(s) $ contains the term $e^{-kTs}$, it is not a rational function of $s$. When terms with $e^{-Ts}$ appear in a transfer function other than a multiplying factor, difficulties arise while taking the inverse Laplace. It is desirable to transfer the irrational function $F^*(s)$ to a rational function for which one obvious choice is:
\begin{equation\*}
z =  e^{Ts}  \Rightarrow \; s=  \frac{1}{T} ln \; z
\end{equation\*}
