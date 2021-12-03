# Differential Operators 

Consider a differential operator that is given in the form:

>$$\begin{align} \mathcal L = p_0(x)\frac{d^n}{dx^n} + p_0\frac{d^{n-1}}{dx^{n-1}} +...+ p_n(x)\end{align}$$

### 3.0.1) Algebra of Operators:
>$$\begin{gather} (\partial_x + v)(\partial_x+w) = \partial_x^2 + w' +(w+v)\partial_x+vw\end{gather}$$

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




### 3.2.3) Boundary Conditions
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

## 3.4) Properties of Hermitian Operators
Infinite set of Eigenfunctions and corresponding eigenvalues: 

>$$\begin{gather} \mathcal L\{u_n(x)\} = \lambda_n u_n(x) \end{gather}$$

The corresponding eigenvalues are real

Eigenfunctions are orthonormal (upon normalization)

>$$\begin{gather} \braket{u_n,u_m} = \int^b_a \omega(x)\overline{u}(x)u(x)dx = \delta_{n,m} \end{gather}$$

The orthonormal basis is complete for any $y(x) \in L_2[a,b]$

>$$\begin{gather} ||y(x) - \sum^N_{n=1}a_nu_n(x)|| \rightarrow_{N \to \infty}\rightarrow 0 \end{gather}$$







