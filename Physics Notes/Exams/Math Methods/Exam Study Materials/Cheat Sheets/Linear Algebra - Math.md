# Linear Algebra
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


### Parallelogram Law Proof

Defined as:
>$$\begin{gather} ||f+g||^2 + ||f-g||^2 = 2||f||^2 + 2||g||^2 \end{gather}$$

Proof:

>$$\begin{gather} ||f+g||^2 = \braket{f+g,f+g} \\ =\braket{f,f}+ \braket{f,g}+ \braket{g,f} + \braket{g,g}\\ = ||f||^2+||g||^2 +\braket{f,g} + \braket{g,f} \\ ||f-g||^2 = \braket{f-g,f-g} \\ =\braket{f,f}+ \braket{f,g}+ \braket{g,f} + \braket{g,g}\\ = ||f||^2+||g||^2 -\braket{f,g} - \braket{g,f} \\ = 2||f||^2 + 2||g||^2 \end{gather}$$

### Triangle Inequality Proof

Defined as: 

$$\begin{gather} ||x + y|| \leq ||x|| + ||y|| \end{gather}$$

Proof:
Assume two real valued vectors $x$ and $y$:

$$\begin{gather} -|x| \leq x \leq |x| \\  -|y| \leq y \leq |y|\\ \end{gather}$$

Add the two equations together:

$$\begin{gather} -|x| + -|y| \leq x + y \leq |x| + |y|\end{gather}$$

Using the properties of inequalities: $|b| \leq a \leftrightarrow -a \leq b \leq a$

We can rewrite the form:
$$\begin{gather} |x + y| \leq |x| + |y| \end{gather}$$
