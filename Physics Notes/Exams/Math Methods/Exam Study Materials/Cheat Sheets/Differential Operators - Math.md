# Differential Operators 

Consider a differential operator that is given in the form:

>$$\begin{align} \mathcal L = p_0(x)\frac{d^n}{dx^n} + p_0\frac{d^{n-1}}{dx^{n-1}} +...+ p_n(x)\end{align}$$

### 3.0.1) Algebra of Operators:
$$\begin{gather} (\partial_x + v)(\partial_x+w) = \partial_x^2 + w' +(w+v)\partial_x+vw\end{gather}$$

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

If $\mathcal L = \mathcal L^\dagger$, $\mathcal D(\mathcal L) = \mathcal D(\mathcal L^\dagger)$, and $Q[u,v]|^b_a = 0$ $(\braket u |\mathcal L v) = \braket{\mathcal Lu|v})$ then $\mathcal L$ is truly self-adjoint or Hermitian. 

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

### 3.3) Boundary Conditions
A property of Truly adjoint operators is that:
$$\begin{gather} \mathcal D(\mathcal L) = \mathcal D(\mathcal L^\dagger) \\ Q[u,v]\Bigg|^b_a =0\end{gather}$$

Where $a$ and $b$ are arbitrary boundaries.

To prove that the domain is the same (and that the boundaries vanish), we use Lagrange's Identity to find when the operator acting on some function is equal to zero.

Consider the following:

The Sturm-Liouville Operator is defined as: 
>$$\begin{gather}\mathcal L = \frac{d}{dx}\left(p_0(x)\frac{d}{dx}\right)+p_2(x) \\x \in [a,b] \\ \omega(x)=1\end{gather}$$

Now we must find the boundary conditions such that $Q = 0$

Begin with Lagrange's Identity:

>$$\begin{gather} \braket{\overline{u}|\mathcal L v} - \braket{\mathcal L^\dagger\overline{u}| v} = 0 \\ \omega[\overline{u} \mathcal L v - v \overline{\mathcal{L}^\dagger u}] = 0\\ \overline{u} \left[\frac{d}{dx}(p_0(x)\frac{d}{dx}v)+p_2(x)v\right] -  v\left[\frac{d}{dx}(p_0(x)\frac{d}{dx}\overline{u})+p_2(x)\overline{u}\right] \\ = \frac{d}{dx}\left[p_0(x)\left(\overline{u}\frac{dv}{dx} - v\frac{d\overline{u}}{dx}\right)\right]\end{gather}$$

Now we must obtain the domain by specifying boundary conditions. Recall that we defined our boundaries as $a$ and $b$. We specify boundary conditions on all functions $u$ and $v$ such that: 

>$$\begin{gather} Q[u,v]\Bigg|_{x=b} - Q[u,v]\Bigg|_{x=a} =0 \\ \\ \overline{u}\frac{dv}{dx}\Bigg|_{x=a} -  \overline{u}\frac{dv}{dx}\Bigg|_{x=b} -v\frac{d\overline{u}}{dx}\Bigg|_{x=a} + v\frac{d\overline{u}}{dx}\Bigg|_{x=b} \end{gather}$$

Now consider the Dirichlet type BC:

>$$\begin{gather} \overline{u}(a) = \overline{u}(b) = 0\Rightarrow v(a) = v(b) = 0 \end{gather}$$

Since each term vanishes, the whole sum vanishes.

Next consider Neumann BC's:

>$$\begin{gather} \frac{d \overline{u}}{dx}\Bigg|_{x=a} = \frac{d \overline{u}}{dx}\Bigg|_{x=b} = \frac{dv}{dx}\Bigg|_{x=a} = \frac{dv}{dx}\Bigg|_{x=a} = 0 \end{gather}$$

Now we assume that each BC is a linear combination of Dirichlet and Neumann, such that:

>$$\begin{gather} \alpha \overline{u}(a) + \beta \overline{u}\ '(a) = 0\Rightarrow \alpha v(a) + \beta v'(a)=0\\ \gamma \overline{u}(b) + \delta \overline{u}\ '(b) = 0\Rightarrow \gamma v(b) + \delta v'(b)=0 \end{gather}$$

Consider then the two terms: 
>$$\begin{gather} \overline{u}(a) v'(a) - v(a) \overline{u}'(a) \\ \overline{u}(a) v'(a)+\frac{\beta}{\alpha}v'(a) \overline{u}'(a) = v'(a)[\overline{u}(a)+\frac{\beta}{\alpha}\overline{u}(a)] = \\ \frac{v'(a)}{\alpha}[\overline{u}(a)+\beta\overline{u}(a)] \Rightarrow  \overline{u}(a) v'(a) - v(a) \overline{u}'(a) = 0 \end{gather}$$

This same process applies to the other two terms evaluated at $x=b$.