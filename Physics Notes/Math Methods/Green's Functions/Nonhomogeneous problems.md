### Definition
Solutions to specific differential equations of the form $\mathcal L y(x) = f(x)$ where $f(x)$ is some given function (source), where $\mathcal L$ is a [[Linear Differential Operator]] under homogeneous boundary condition or nonhomogeneous boundary condition.

The general method to solve such equations is called the Green's function method. 

### Recap of basic arithmetic
$$\begin{gather} mx=a \end{gather}$$

The cases are: $a \neq 0$ (nonhomogeneous), we can have either $m=0$ so there is no solution or $m\neq0$ and the single solution is $x = m^{-1}a$; $a = 0$ (homogeneous) the first is if $m = 0$ then there are infinitely many solutions ($x$ is any number) or $m\neq0$ where only $x = 0$ is the solution.

### Fredholm Alternative

Now we can consider the analogous equation in $c^n$ where $$\begin{gather}x\rightarrow\vec X = \begin{bmatrix}x_1\\ \vdots \\ x_n\end{bmatrix},a\rightarrow \vec a = \begin{bmatrix}a_1\\ \vdots \\ a_n\end{bmatrix}\end{gather}$$

and 

$$\begin{gather}m \rightarrow \vec M = \begin{bmatrix} m_{11} & \ldots &m_{1n} \\ \vdots & \ddots & \vdots \\m_{n1} & \ldots &m_{nn}\end{bmatrix} \end{gather}$$

now the invertability condition is whether $\overleftrightarrow M^{-1}$ exists. Namely, whether or not there is matrix $\overleftrightarrow K$ such that 

$$\begin{gather}\overleftrightarrow M \cdot \overleftrightarrow K = \overleftrightarrow I \rightarrow  \begin{cases}  \overleftrightarrow M^{-1} = \overleftrightarrow K & \text{Ker}(\overleftrightarrow M) = 0 & \text{det} \overleftrightarrow M \neq 0 \\ \overleftrightarrow M \text{is not-invertible} & \text{Ker}(\overleftrightarrow M) \neq 0 & \text{det} \overleftrightarrow M = 0\end{cases} \end{gather}$$

Useful links: [[Determinant]], [[Kernel]]

Now consider: 
$$\begin{gather} \overleftrightarrow M \cdot \vec x = \vec a  \end{gather}$$

#### For the case $\det \overleftrightarrow M = 0$ (non-invertible): 

$\vec a = 0$ (homogeneous) infinitely many solutions, linearly independent solutions are called zero modes, number of independent solutions defines [[Dimension]] of the linear [[Subspace]] dim (Ker($\overleftrightarrow M$)) $\leq n$ and dim (Ker($\overleftrightarrow M$)) = dim(Ker($\overleftrightarrow M^\dagger$))

$\vec a \neq 0$ (nonhomogeneous) solutions exist only if $\vec{a} \not \in \text{Ker} ({\overleftrightarrow M^\dagger})$ i.e. $\braket{\vec a | \vec y} = 0$  $\forall \vec y \in \text{Ker}(\overleftrightarrow M^\dagger)$, in such a case there are infinitely many solutions of the form: $$\begin{gather} \vec x = \vec x_0 + \sum_{n=1}^{\text{dim(Ker}\overleftrightarrow M)} \alpha_j\vec a_j \end{gather}$$ where $\{\vec a_j\}$ are [[Basis Vectors]] for Ker($\overleftrightarrow M$)

#### For the case $\det \overleftrightarrow M \neq 0$ (invertible)

$\vec a = 0$ (homogeneous) only solution is $\vec x = 0$ 

$\vec a \neq 0$ (non-homogeneous) single solution $\vec X = \overleftrightarrow M^{-1} \cdot \vec a$