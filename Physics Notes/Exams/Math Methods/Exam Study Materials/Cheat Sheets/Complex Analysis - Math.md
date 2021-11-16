# 1) Complex Analysis
## 1.1) Cauchy Formula
If a function $f(z)$ is analytic in $\Omega$ then for any $z_0 \in \Omega$
>$$\begin{align} f(z_0) = \frac{1}{2 \pi i}\oint_\Gamma \frac{f(z)}{z - z_0}dz \end{align}$$

where $\Gamma$ is any closed contour in $\Omega$ that encloses $z_0$


## 1.3) Analytic Continuation
Provides a way to extend the domain over which a complex function is defined. 

Think about it like this, you can Taylor expand around a point until you hit a singularity, then you Taylor expand around that point, and so on and so forth.

## 1.4) Residue

The Coefficient $a_{-1}$ in the Laurent expansion: $\text{Res}[f,z_0] \equiv a_{-1}$

Non-Essential Singularity of order m allows us to compute the residue easily by:

>$$\begin{align} g(z) = (z-z_0)^m f(z) = (z-z_0)^m\sum^\infty_{n=-m} a_m(z-z_0)^n = \sum^\infty_{n=0} a_{n-m}(z-z_0)^n \end{align}$$

Hence: 
>$$\begin{gather} a_{n-m} = \frac{1}{n!}g^n(z_0) = a_n=\frac{1}{(n+m)!}g^{(n+m)}(z_0)\\ Res[f,z_0] = a_{-1}=\frac{1}{(m-1)!}g^{(m-1)}(z_0)\end{gather}$$

Where $m$ is the order of the pole

## 1.5) Residue Theorem
>$$\begin{align} \oint_\Gamma f(z)dz = 2\pi i \sum_{z_0} \text{Res}[f,z_0] \end{align}$$



## 1.7) Jordan's Lemma
Consider a complex-valued, continuous function $f$ defined on a semicircular contour or positive radius $R$ lying in the upper half-plane centered at the origin. If the function $f$ is of the form: 
>$$\begin{align}f(z) = e^{iaz}g(z) \end{align}$$
where $a$ is a positive parameter.

Then: 
>$$\begin{align} \lim_{R\to\infty}\int_{C_R} f(z)dz = 0 \end{align}$$

### 1.7.1) Application
If we have some holomorphic function $f(z)$ on the upper half plane. Consider a semi-circular contour defined by $C_1$ along the real line, and $C_2$ a semicircle in the positive plane from $0 \to \pi$

>$$\begin{gather} \oint_C f(z)dz  = \int_{C_1}f(z)dz + \int_{C_2}f(z)dz \\ \int_{C_2} f(z)dz = \int ^R_{-R}f(x)dx \\ \oint_C f(z)dz = 2\pi i \sum^n_{k=1} \text{Res}(f,z_k)  \end{gather}$$

The contour over $C_1$ vanishes leaving: 
> $$\begin{gather}\int^\infty_{-\infty} f(x)dx = 2\pi i\sum^n_{k=1} \text{Res}(f,z_k) \end{gather}$$

## 1.8) Principal Value Theorem

For an integral that diverges, we redefine the integral as a sum of two integrals, with one approaching from the left to the point, then from the point to the right.