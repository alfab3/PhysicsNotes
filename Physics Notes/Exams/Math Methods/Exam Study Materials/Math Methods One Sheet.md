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


##### Sector Contour $(0, \infty)$
An integral on the real range $(0,\infty)$ that lacks the symmetry needed to extend the integration range to $(-\infty,\infty)$

Consider: 
>$$\begin{align} I = \int^\infty_0 \frac{dx}{x^3+1}  \end{align}$$

Solve for the pole:
>$$\begin{gather} x^3+1=0 \\ x^3 = -1 \\  x^3 =e^{i\pi} \\ x = e^{i\pi/3}\end{gather}$$

So now we can set the sector contour to include this pole, we choose the angle: $\theta = 2\pi/3$

##### Rectangular contour
Solve for poles, if when you take $R \to \infty$ a semicircle will enclose infinitely many poles, you must use a rectangular contour.

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

For an integral that diverges, we redefine the integral as a sum of two integrals, with one approaching from the left to the point, then from the point to the right.


# 2)Linear Algebra
## Review
### Inner Product 
Mapping $R^n \rightarrow R$ for each $\vec v \in R^n$ we  we can define: 

>$$\begin{align} F_{\vec v}(\vec u) = \vec v \cdot \vec u = \vec u \cdot \vec v \in R \end{align}$$

### Norm
Length of a vector and distance between two vectors

>$$\begin{gather} |\vec v_1 - \vec v_2| = \sqrt{(\vec v_1 - \vec v_2) \cdot (\vec v_1 - \vec v_2)} = \sqrt{(\vec v_1) \cdot (\vec v_1) +(\vec v_2)(\vec v_2) - 2 (\vec v_1\vec v_2)} \\ \text{norm}(\vec v) = ||\vec v|| = \sqrt{\vec{v}\cdot\vec{v}}\end{gather}$$

### Basis
For a vector space of dimension $n$ there is a set of $n$ vectors $\{\vec v_j\}^n_{j=1}$ such that for any vector in the space we can write:

>$$\begin{align}\vec v = \sum^n_{j=1} a_j\cdot \vec v_j \end{align}$$

#### Orthogonal Basis 

If $\vec{v}_j \cdot \vec{v}_i = 0$ for any $1 \leq i \neq j \leq n$  then the set of coefficients is unique.

#### Orthonormal Basis
Orthogonal basis with the additional property that $|\vec{v}_j =1 \forall 1 \leq j \leq n$ 

Therefore: $\vec u_i \cdot \vec u_j = \delta_{ij}$

### Gram-Schmidt Algorithm 
Every basis can be made orthonormal by this process:

>$$\begin{gather} \vec v'_1 = \frac{\vec v_1}{||\vec v_1||} \\ \vec v_ 2' = \frac{(\vec v_2 - (\vec v_2 \cdot \vec v_1 ') \cdot \vec v_1')}{||(\vec v_2 - (\vec v_2 \cdot \vec v_1 ') \cdot \vec v_1')||}\end{gather}$$
### Parseval Theorem

Consider $\vec v$ in vector space of dimension $n$ and an orthonormal basis $\{\vec v_1\}^n$ such that $\vec v = \sum^n_{j=1}a_j \vec v _j$

Then 
>$$\begin{gather}||\vec v||^2=\sum^n_{j=1}a_j^2\end{gather}$$
## Best Approximation
Consider $\vec v$ in vector space of dimension $n$ and an orthonormal basis $\{\vec v_j\}^n$ such that $\vec v= \sum^n_{j=1} a_j\vec{v}_j$. Consider a subset $\{\vec{v}_j\}^k_{j=1}$ with $k < n$ 

Then the best approximation for $\vec v$ with $\{\vec{v}_j\}^k_{j=1}$ is $\vec v = \sum^k_{j=1} a_j \vec v_j$

Define 
>$$\begin{align} \text{err}[b_1 - b_k] = ||\vec v - \sum^k_{j=1}b_j \vec v_j||\end{align}$$

Then 
>$$\begin{align}\text{min  err}[b_1 - b_k] = ||\sum^N_{j = k+1} a_j \vec v_j\ ||\end{align}$$

## Delta Functions

The identity operator in $\infty$-dim space is the Dirac-delta "function"

>$$\begin{gather}I\{f(x)\} = \int^b_a \delta(x-y) f(y)dy = f(x) \end{gather}$$

Derivative of the Delta Function: $\frac{d}{dx}\delta(x)$ 
>$$\begin{gather} \int^b_a\left[\frac{d}{dx} \delta(x-y) \right]f(y) dy = -\int^b_a f(y) \frac{d}{dy}\delta(x-y) = -\delta(x-y)f(y)\Bigg|^b_a + \int^b_a f'(y) \delta(x - y) \\ = f'(x)\end{gather}$$

Explanation of the first step:
>$$\begin{gather} \frac{d}{dx}\delta(x-y) = \frac{d}{d(x-y)}\delta(x-y)\frac{d(x-y)}{dx} = \delta'(x-y) \\ \frac{d}{dy}\delta(x-y) = \frac{d}{d(x-y)}\delta(x-y)\frac{d(x-y)}{dx} = -\delta'(x-y) \\ \frac{d}{dx}\delta(x-y) = -\frac{d}{dy}\delta(x-y)90\end{gather}$$


# 3) Differential Operators 

Consider a differential operator that is given in the form:

>$$\begin{align} \mathcal L = p_0(x)\frac{d^n}{dx^n} + p_0\frac{d^{n-1}}{dx^{n-1}} +...+ p_n(x)\end{align}$$

## 3.1)Linear Algebra Review: n x n square matrices
#### Non - Commutation: 
>$$\begin{gather} [A,B] \neq 0 \end{gather}$$

#### Eigenvalues and Eigenvectors
Square matrices may have solutions of the following equation:
>$$\begin{align} \overleftrightarrow{A} \vec v = \lambda \vec v \end{align}$$

Where $\lambda$ is the eigenvalue and $\vec v$ is the eigenvector

#### Symmetric real matrices
>$$\begin{gather}A_{ij} = A_{ji} \\ A_{ij} = \overline{A}_{ji} \end{gather}$$

have $n$ real eigenvalues

#### Eigenvectors as Orthonormal Basis
Normalized eigenvectors $\{\vec v_j\}^n_{j=1}$ of a Hermitian matrix form an orthonormal basis for n - dim vector space.

>$$\begin{align} \vec v = \sum^n_{j=1} b_j \cdot \vec v_j \end{align}$$ 

#### Orthogonal Real Matrices 

$\overleftrightarrow{R}$ such that $R_{ij} \cdot R_{ji} = \delta_{ij}$ and more generally unitary complex matrices $\overleftrightarrow{U}$ such that $U_{ij} \cdot U_{ji} = \delta_{ij}$ rotate matrices

Specifically the matrix constructed by the eigenvectors $\{\vec v_j\}^n_{j=1}$ of a Hermitian matrix $\overleftrightarrow A$ form a unitary matrix $\overleftrightarrow U$ that diagonalizes the matrix $\overleftrightarrow A$ 
>$$\begin{gather} \overleftrightarrow U = (\vec v_1 \;\; \vec v_2 \;\; ... \;\; \vec v_n) \\ \overleftrightarrow{U}^\dagger \overleftrightarrow A \overleftrightarrow U = \overleftrightarrow D \\ \overleftrightarrow D = \begin{bmatrix} \lambda_1 & 0 \\ 0 & \lambda_2 \end{bmatrix} \end{gather}$$

#### Square Matrices to Linear Differential Operator

Operators do not commute


## 3.2)Lagrange Identity, Adjoint, Boundary Conditions
For a given linear differential operator $\mathcal L$ of order $n$, the formal adjoint $\mathcal L^\dagger$ is defined by the Lagrange identity:

>$$\begin{gather}\braket{u|\mathcal L v}  - \braket{ \mathcal L^\dagger u| v} = Q[u,v] \Bigg|^b_a  \\ \int^b_a \overline{u(x)} \mathcal L v(x)\omega(x) - \int^b_a \overline{\mathcal L^\dagger u(x)}v(x)\omega(x) = Q[u,v] \Bigg|^b_a\end{gather}$$

$Q$ is a function of $u(x),v(x)$ and their derivatives of $(n-1)$ order. When $\mathcal L = \mathcal L^\dagger$ the operator is formally self-adjoint. 

If $\mathcal L = \mathcal L^\dagger$, $\mathcal D(\mathcal L) = \mathcal D(\mathcal L^\dagger)$, and $Q[u,v]|^b_a = 0$ then $\mathcal L$ is truly self-adjoint or Hermitian. 

### 3.2.1)Find Formal Adjoint
Use Lagrange identity
Integrate by parts to move derivatives from $u$ to $v$

### 3.2.2) Integration by parts technique

Consider an operator $\mathcal L = -\frac{d^2}{dx^2}$

We want to apply this to Lagrange's identity, where it will be acting on $v$ and we are going to "move" the operator to $u$:

>$$\begin{gather} \int \overline{u} \mathcal L v dx= -\int \overline{u} \frac{d^2v}{dx^2} dx\end{gather}$$

Now we set $u = u$ and $v = \frac{d}{dx}v$ and apply integration by parts which is defined as:

>$$\begin{gather} \int udv = uv - \int vdu  \end{gather}$$

Applying this to the right hand side of our above equation 
>$$\begin{gather} -\int \overline{u} \frac{d^2v}{dx^2} dx = \overline{u}\frac{dv}{dx} - \int \frac{dv}{dx}\frac{d\overline{u}}{dx}dx\end{gather}$$

Now we must apply the integration by parts technique once more. $\overline{u} = \frac{d\overline{u}}{dx}$ and $v = v$

>$$\begin{gather} \overline{u}\frac{dv}{dx} - \int \frac{dv}{dx}\frac{d\overline{u}}{dx}dx = \overline{u}\frac{dv}{dx} + \frac{d\overline{u}}{dx}v - \int \frac{d^2u}{dx^2}vdx \\ =-\left(\overline{u} \frac{dv}{dx} - \frac{d\overline{u}}{dx}v\right)+\int v\mathcal L^\dagger\ \overline{u}dx \end{gather}$$

We have arrived at the (formal) adjoint operator.

Now let us consider a weight function $\omega(x) > 0$

Consider the momentum operator case: 

>$$\begin{gather} \mathcal L = -i\frac{d}{dx} \end{gather}$$

Utilizing Lagrange's identity we can see that:

>$$\begin{gather} \int \omega \overline{u} \mathcal L v = \int \omega \overline{u} \left(-i\frac{d}{dx} v\right) \end{gather}$$

Using integration by parts we define $u = \omega u$ and $v = v$

>$$\begin{gather}\int \omega \overline{u} \left(-i\frac{d}{dx} v\right) = -i\omega \overline{u} v + \int iv\frac{d}{dx}(\overline{u} \omega) \end{gather}$$

Now this can be written in derivative form as:
>$$\begin{gather} \omega \overline{u} \left(-i\frac{d}{dx} v\right) = -i\frac{d}{dx}(\omega \overline{u} v) +  iv\frac{d}{dx}(\overline{u} \omega) \end{gather}$$

Since $\omega$ is dependent on $x$ then we must apply product rule:

>$$\begin{align} -i\frac{d}{dx}(\omega \overline{u} v) +  iv\frac{d}{dx}(\overline{u} \omega) = -i\frac{d}{dx}(\omega \overline{u} v) + iv\omega\frac{d}{dx}(\overline{u}) + iv\overline{u}\frac{d}{dx}(\omega) \end{align}$$

The integration by parts is complete.
#### Example 1: First Order $\omega(x) = 1$
Find adjoint of the Linear Differential Operator: $\mathcal L = -i \frac{d}{dx}$ with $\omega(x) = 1$

>$$\begin{gather} \overline{u}(\mathcal L v) = \overline u\left(-i\frac{d}{dx} v\right) = \left(i\frac{d}{dx} \overline{u}\right)v - i\frac{d}{dx}(\overline uv) = \overline{\left(-i\frac{d}{dx} u \right)} v + \frac{d}{dx}(-i \ \overline{u} v) \\ \mathcal L^\dagger = -i\frac{d}{dx} =\mathcal L^\dagger \\ Q[u,v] = -i \ \overline u v\end{gather}$$

Therefore $\mathcal L = -i\frac{d}{dx}$ is formally self-adjoint

#### Example 2: Second Order Diff eq $\omega(x) = 1$
>$$\begin{align} \mathcal L = p_0(x)\frac{d^2}{dx^2} + p_0\frac{d}{dx} + p_2(x) \end{align}$$

We use a similar approach and find that:

>$$\begin{gather} \mathcal L^\dagger = p_0(x)\frac{d^2}{dx^2}+(2p_0'(x)-1)\frac{d}{dx} + [p_o''(x) - p_1'(x) + p_2(x)] \end{gather}$$

Formal self-adjointness with $\omega(x)$ of above operator is only if $p_0'(x) = p_1(x)$, $p_0''(x) = p_1'(x)$.

$\mathcal L$ is self-adjoint with $\omega(x) = 1$
>$$\begin{gather} \mathcal L = \frac{d}{dx}\left(p_0 \frac{d}{dx}\right) + p_2(x)\end{gather}$$

This is called the Sturm-Liouville Operator

Any 2nd order diff op is formally-self - adjoint with a weight function: 

>$$\begin{gather} \omega(x) = \frac{1}{p_0(x)} e^{\int^x_a\left(\frac{p_1(x')}{p_0(x')}\right)dx'}\end{gather}$$

#### Example 3: Momentum Operator $\omega(x) > 0$

Consider the momentum linear operator: $\mathcal L -i \frac{d}{dx}$ for functions on the interval $x \in [a,b]$. Find the Adjoint operator $\mathcal L$

Start with the Lagrange identity:

>$$\begin{gather} \omega(x)(\overline u \mathcal L v - v\overline{\mathcal L u}) = \frac{d}{dx} Q(u,v) \\ \omega \overline u\left(- i \frac{d}{dx}\mathcal L v\right) = \omega \overline u\left( -i \frac{d}{dx}v\right)\end{gather}$$

Now we "move" the derivative operator to $\overline u$

>$$\begin{gather} \omega \overline u \left(-i \frac{d}{dx} v\right) = -i\frac{d}{dx}(\omega \overline u v)  + v i \frac{d}{dx}(\omega \overline u) = -i\frac{d}{dx}(\omega \overline u v) + \omega v i \frac{d}{dx}\overline u + \overline u v i \frac{d}{dx}\omega \end{gather}$$

Let us now write $\mathcal L^\dagger = \mathcal L^\dagger_1 + \mathcal L_2^\dagger$

such that: 
>$$\begin{gather}\omega v i \frac{d}{dx}\overline u + \overline u v i \frac{d}{dx} = \omega v \overline{\mathcal L^\dagger_1 u} + \omega v \overline{\mathcal L^\dagger_2 u}  \end{gather}$$

It is easy to see that: 
>$$\begin{gather} \overline{\mathcal L^\dagger_1 u} = i\frac{d}{dx} \overline u = \overline{-i \frac{d}{dx} u} \Rightarrow \mathcal L^\dagger_1 = -i\frac{d}{dx} = \mathcal L \end{gather}$$

Now we solve for the second term:
>$$\begin{gather} \omega v \overline{\mathcal{L}^\dagger u} = \overline{u}v i \frac{d}{dx} \omega = \omega v i \frac{1}{\omega} \frac{d\omega}{d x}\overline{u} = \omega v \left(\overline{-i \frac{1}{\omega}\frac{d\omega}{d x} u}\right) \\ \overline{\mathcal L^\dagger_2 u} = \overline{-i\frac{1}{\omega}\frac{d\omega}{dx}u}\\ \mathcal L_2^\dagger = - i\frac{1}{\omega}\frac{d\omega}{dx} = -i \frac{d}{dx}(\ln \omega) \\ \mathcal L^\dagger = -i\frac{d}{dx} - i\frac{d}{dx}\ln\omega \end{gather}$$

#### Example 4: Second Order Operator
>$$\begin{align} \mathcal L = p_0(x)\frac{d^2}{dx^2} + p_0\frac{d}{dx} + p_2(x) \end{align}$$

With the corresponding weight function: 
>$$\begin{gather} \omega(x) = \frac{1}{p_0(x)} e^{\int^x_a\left(\frac{p_1(x')}{p_0(x')}\right)dx'}\end{gather}$$

Begin with 
>$$\begin{gather} \omega\left(\overline{u} \mathcal L v - v \overline{\mathcal L^\dagger u}\right) = - \frac{d}{dx} Q(u,v) \end{gather}$$

with $\mathcal L^\dagger = \mathcal L$



### 3.2.2) True Self-Adjoint operator
>$$\begin{gather} \mathcal L ^ \dagger = \mathcal L \\ \mathcal D(\mathcal L^\dagger) = \mathcal D(\mathcal L) \end{gather}$$
# 4)Green's Functions

## Fourier Transform

Transform
>$$\begin{gather} f(x) = \int^\infty_{-\infty} \frac{dk}{2\pi} g(k)e^{ikx}  \end{gather}$$

Inverse Transform
>$$\begin{align} g(k) = \int^\infty_{-\infty} f(x)e^{-ikx}dx \end{align}$$

## Solving for Green's Functions
#### Example 1: Helmholtz problem
Fourier transform is given by:

$$\begin{gather} \tilde h(k,y) = \tilde h(k,0) e^{-\sqrt{k^2+l_c^2}|y|} \end{gather}$$