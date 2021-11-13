# 1) Complex Analysis
## 1.1) Cauchy Formula
If a function $f(z)$ is analytic in $\Omega$ then for any $z_0 \in \Omega$
>$$\begin{align} f(z_0) = \frac{1}{2 \pi i}\oint_\Gamma \frac{f(z)}{z - z_0}dz \end{align}$$

where $\Gamma$ is any closed contour in $\Omega$ that encloses $z_0$

## 1.2) Laurent Series
If $f(z)$ is analytic throughout the region there exists a series expansion in terms of positive and negative powers of (z - a) (where a is the center of the region)

>$$\begin{align} f(z) = \sum_{k=0}^\infty a_k(z-a)^k + \sum^\infty_{k=1}b_k(z-a)^{-k} \end{align}$$

where 
>$$\begin{gather} a_k = \frac{1}{2\pi i}\oint_{K_1} \frac{f(\zeta) d\zeta}{(\zeta - a)^{k+1}} \\ b_k = \frac{1}{2\pi i}\oint_{K_2}(\zeta - a)^{k-1}f(\zeta)d \zeta\end{gather}$$

### 1.2.1) L'Hopital's Rule
In the case where we find a derivative (or more specifically a limit) to give us: $\frac{0}{0}$ we utilize L'Hopital's Rule
>$$\begin{align} \lim_{x \to c} \frac{f(x)}{g(x)} =  \lim_{x \to c} \frac{f'(x)}{g'(x)}\end{align}$$

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

## 1.6) Contour Integration (Residue Calculus)
Given an analytic function, the process of evaluating an integral by use of a path in the complex plane.

### 1.6.1)Method of Evaluation 
#### 1.6.1.1) Define the contour

##### Rational Function 
>$$\begin{align} \int^\infty_{-\infty} F(x)dx \end{align}$$

where $F(x)$ is a rational function. 
Consider $\oint_C F(z)dz$ along a contour $C$ consisting of the line along the $x$ axis from $-R$ to $+R$ and the semicircle $\Gamma$ above the x axis having this line as diameter. Then, let $R \to \infty$. If $F(x)$ is an even function, this can be used to evaluate $\int^\infty_0 F(x)dx$

##### Rational Function with sine or cosine
>$$\begin{align}\int^{2\pi}_0 G(\sin \theta, \cos \theta)d\theta \end{align}$$

Where $G(\sin\theta, \cos\theta)$ is a rational function of $\sin \theta$ and $\cos \theta$

Let $z = e^{i\theta}$. Then $\sin \theta = (z -z^{-1})/2$, $\cos \theta = (z + z^{-1})/2$ and $dz = ie^{i\theta} d\theta$ or $d\theta = dz/iz$. The given integral is equivalent to $\oint_C F(z)dz$ where $C$ is the unit circle with center at the origin.

##### Semi-circle slice contour 
This case is a little tricky, start with the semi-circle case and see how it behaves when $R \to \infty$. 

##### Sector Contour $(0, \infty)$
An integral on the real range $(0,\infty)$ that lacks the symmetry needed to extend the integration range to $(-\infty,\infty)$

Consider: 
>$$\begin{align} I = \int^\infty_0 \frac{dx}{x^3+1}  \end{align}$$

Solve for the pole:
>$$\begin{gather} x^3+1=0 \\ x^3 = -1 \\  x^3 =e^{i\pi} \\ x = e^{i\pi/3}\end{gather}$$

So now we can set the sector contour to include this pole, we choose the angle: $\theta = 2\pi/3$

##### A pole on the Contour

Example: 
>$$\begin{align} I = \int^{\infty}_{-\infty} \frac{\cos x}{x}dx\end{align}$$

Use a semicircle that avoids the singularity (Annulus)

##### Branch Cuts

We can construct a contour around the discontinuity to solve the integral. Example:
>$$\begin{align} J = \int_C \frac{\ln z dz}{z^3 +1}\end{align}$$

#### 1.6.1.2) Rewrite integral
The contour integral now separates into integrals for each segment:

>$$\begin{align}\oint_C = \int_1+\int_2+\ ...\ +\int_n \end{align}$$

#### 1.6.1.3) Evaluate
Residue Theorem
Jordan's Lemma



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

# 2)Linear Algebra
## Best Approximation
Consider $\vec v$ in vector space of dimension $n$ and an orthonormal basis $\{\vec v_j\}^n$ such that $\vec v= \sum^n_{j=1} a_j\vec{v}_j$. Consider a subset $\{\vec{v}_j\}^k_{j=1}$ with $k < n$ 

Then the best approximation for $\vec v$ with $\{\vec{v}_j\}^k_{j=1}$ is $\vec v = \sum^k_{j=1} a_j \vec v_j$

Define 
$$\begin{align} \text{err}[b_1 - b_k] = ||\vec v - \sum^k_{j=1}b_j \vec v_j||\end{align}$$

Then $$\begin{align}\text{min  err}[b_1 - b_k] = ||\sum^N_{j = k+1} a_j \vec v_j ||\end{align}$$

## Delta Functions
# 3) Differential Operators

Consider a differential operator that is given in the form:

>$$\begin{align} \mathcal L = p_0(x)\frac{d^n}{dx^n} + p_0\frac{d^{n-1}}{dx^{n-1}} +...+ p_n(x)\end{align}$$

## 3.1)Lagrange Identity, Adjoint, Boundary Conditions
For a given linear differential operator $\mathcal L$ of order $n$, the formal adjoint $\mathcal L^\dagger$ is defined by the Lagrange identity:

>$$\begin{gather}\braket{u|\mathcal L v}  - \braket{ \mathcal L^\dagger u| v} = Q[u,v] \Bigg|^b_a  \\ \int^b_a \overline{u(x)} \mathcal L v(x)\omega(x) - \int^b_a \overline{\mathcal L^\dagger u(x)}v(x)\omega(x) = Q[u,v] \Bigg|^b_a\end{gather}$$

$Q$ is a function of $u(x),v(x)$ and their derivatives of $(n-1)$ order. When $\mathcal L = \mathcal L^\dagger$ the operator is formally self-adjoint. 

If $\mathcal L = \mathcal L^\dagger$, $\mathcal D(\mathcal L) = \mathcal D(\mathcal L^\dagger)$, and $Q[u,v]|^b_a = 0$ then $\mathcal L$ is truly self-adjoint or Hermitian. 

### 3.1.1)Find Formal Adjoint
Use Lagrange identity
Integrate by parts to move derivatives from $u$ to $v$

### 3.1.2)Domain

# 4)Green's Functions
