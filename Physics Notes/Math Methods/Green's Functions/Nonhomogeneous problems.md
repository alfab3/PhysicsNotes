## Definition
Solutions to specific differential equations of the form $\mathcal L y(x) = f(x)$ where $f(x)$ is some given function (source), where $\mathcal L$ is a [[Linear Differential Operator]] under homogeneous boundary condition or nonhomogeneous boundary condition.

The general method to solve such equations is called the Green's function method. 

## Recap of basic arithmetic
$$\begin{gather} mx=a \end{gather}$$

The cases are: $a \neq 0$ (nonhomogeneous), we can have either $m=0$ so there is no solution or $m\neq0$ and the single solution is $x = m^{-1}a$; $a = 0$ (homogeneous) the first is if $m = 0$ then there are infinitely many solutions ($x$ is any number) or $m\neq0$ where only $x = 0$ is the solution.

## Fredholm Alternative

Now we can consider the analogous equation in $c^n$ where $$\begin{gather}x\rightarrow\vec X = \begin{bmatrix}x_1\\ \vdots \\ x_n\end{bmatrix},a\rightarrow \vec a = \begin{bmatrix}a_1\\ \vdots \\ a_n\end{bmatrix}\end{gather}$$

and 

$$\begin{gather}m \rightarrow \vec M = \begin{bmatrix} m_{11} & \ldots &m_{1n} \\ \vdots & \ddots & \vdots \\m_{n1} & \ldots &m_{nn}\end{bmatrix} \end{gather}$$

now the invertability condition is whether $\overleftrightarrow M^{-1}$ exists. Namely, whether or not there is matrix $\overleftrightarrow K$ such that 

$$\begin{gather}\overleftrightarrow M \cdot \overleftrightarrow K = \overleftrightarrow I \rightarrow  \begin{cases}  \overleftrightarrow M^{-1} = \overleftrightarrow K & \text{Ker}(\overleftrightarrow M) = 0 & \text{det} \overleftrightarrow M \neq 0 \\ \overleftrightarrow M \text{is not-invertible} & \text{Ker}(\overleftrightarrow M) \neq 0 & \text{det} \overleftrightarrow M = 0\end{cases} \end{gather}$$

Useful links: [[Determinant]], [[Kernel]]

Now consider: 
$$\begin{gather} \overleftrightarrow M \cdot \vec x = \vec a  \end{gather}$$

### For the case $\det \overleftrightarrow M = 0$ (non-invertible): 

$\vec a = 0$ (homogeneous) infinitely many solutions, linearly independent solutions are called zero modes, number of independent solutions defines [[Dimension]] of the linear [[Subspace]] dim (Ker($\overleftrightarrow M$)) $\leq n$ and dim (Ker($\overleftrightarrow M$)) = dim(Ker($\overleftrightarrow M^\dagger$))

$\vec a \neq 0$ (nonhomogeneous) solutions exist only if $\vec{a} \not \in \text{Ker} ({\overleftrightarrow M^\dagger})$ i.e. $\braket{\vec a | \vec y} = 0$  $\forall \vec y \in \text{Ker}(\overleftrightarrow M^\dagger)$, in such a case there are infinitely many solutions of the form: $$\begin{gather} \vec x = \vec x_0 + \sum_{n=1}^{\text{dim(Ker}\overleftrightarrow M)} \alpha_j\vec a_j \end{gather}$$ where $\{\vec a_j\}$ are [[Basis Vectors]] for Ker($\overleftrightarrow M$)

### For the case $\det \overleftrightarrow M \neq 0$ (invertible)

$\vec a = 0$ (homogeneous) only solution is $\vec x = 0$ 

$\vec a \neq 0$ (non-homogeneous) single solution $\vec X = \overleftrightarrow M^{-1} \cdot \vec a$

## Relation to Differential Operators

Consider $\mathcal L y(\vec x) = f(\vec x)$ with $f(\vec x) \neq 0$ with some boundary condition. 

Then $\mathcal L$ is "invertible" if it has no zero modes. Namely, no solutions to $\mathcal Ly(\vec x) = 0$ (except the trivial one: $y(\vec x) = 0$) And $\mathcal L$ is non-invertible if it does have zero modes. 

Fredholm alternative (just like for finite dim matrices)

If $\mathcal L$ is invertible then $\mathcal Ly(\vec x) = f(\vec x)$ has a unique solution that can be written formally as $$\begin{gather} y(\vec x) = \mathcal L^{-1}f(\vec x) \end{gather}$$.

If $\mathcal L$ is "non-invertible" then $\mathcal L y(\vec x) = f(\vec x)$ has a solution is  $\braket{f(\vec x)|u(\vec x)} = 0$ ([[Inner Product]]) for all zero-modes of $\mathcal L^\dagger$, i.e. $\vec u(x)$ such that $\mathcal L^\dagger u(\vec x) = 0$

#### Example: 
Consider $\mathcal L = -\frac{d^2}{dx^2}$ where $x \in (0,1)$ with boundary condition $$\begin{gather}\frac{dy}{dx}\bigg|_{x=0} = \frac{dy}{dx}\bigg|_{x=1} = 0\end{gather}$$ consider the equation $$\begin{gather} -\frac{d^2y}{dx^2} = f(x) \end{gather}$$with some $f(x) \neq 0$ Is there a solution to this equation.

Answer: To apply Fredholm alternative we need to consider $\mathcal L^\dagger$ we showed that $\mathcal L^\dagger = \mathcal L$ and $D(\mathcal L^\dagger) = D(\mathcal L)$ (so $\mathcal L$ is self-adjoint)

Now, $\mathcal L^\dagger$ has a zero mode $u(x)=1$