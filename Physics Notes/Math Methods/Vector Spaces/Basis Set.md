We need two concepts to begin this [[Linear Independence]] and [[Span]].
For example: $\hat{e}_x, \; \hat{e}_y$ are linearly independent but do not span  $\mathbb{R}^3$. $\hat{e}_x, \; \hat{e}_y, \; \hat{e}_z$: span the space, and are linearly independent. Here's a set $\hat{e}_x, \; \hat{e}_y, \; \hat{e}_z, \; \hat{e}_x + \hat{e}_y$ that spans the space and is not linearly independent. $\hat{e}_x, \; \hat{e}_y + \hat{e}_x, \; \hat{e}_z + \hat{e}_y + \hat{e}_x$: this spans $\mathbb{R}^3$ and is linearly independent. A set of vectors that are linearly independent and [[Span]] the [[linear vector spaces]] form a basis set in the linear vector space. [[Span]] does not imply linear independence and vice versa, you need both of them to form a basis([[Basis Vectors]]). If the basis consists of mutually orthogonal [[Vectors]] and each of them have magnitude 1 then we call it an orthonormal basis this would be written as:
$$\begin{equation}
    \braket{\phi_i|\phi_j} = \delta_{i j}
\end{equation}$$
Orthonormal basis sets are the convention but they are NOT required by any means. As long as a basis set is linearly independent and spans the space you have a basis set. The number of vectors in the basis set in our linear vector space is called the dimensionality of the space. For example in 3D euclidean space you need 3 linearly independent [[Basis Vectors]] that [[Span]] the space. The dimension of $V$ is the number of vectors in a basis set. If there is no finite basis set then the Linear Vector Space is infinitely dimensional. $\mathbb{R}^2$ has a finite basis set because any vector can be described as a [[Linear Combination]] of the two [[Basis Vectors]].

Let's look at $\mathbb{R}^n$ and try to make it infinite. If we have:
$$\begin{gather}\mathbb{R}^n =
\begin{bmatrix}
        x_1\\
        x_2\\
		\vdots\\
		x_n
\end{bmatrix}
=\ket{\phi}\end{gather}$$

$$\begin{gather}\braket{\phi | \phi} = ||\phi||^2 = \sum_{i=1}^n |x_i|^2\end{gather}$$

It is not clear that this will converge when $n$ goes to infinity. So we have to put in a condition that the [[Vectors]] have finite length. 
$$\sum^\infty_{i=1} |x_i|^2 < \infty $$ So with this condition we can now work with infinite dimensions. This space has a special name, the Linear Vector Space of square-summable sequences, and it is denoted by $l_2$. For example $$x_r = \frac{1}{r^\epsilon}$$ is in $l_2$ as long as $\epsilon > \frac{1}{2}$. 

What is the advantage of writing a basis?

Well if you start with an arbitrary basis (one that is not orthonormal) you can make it orthonormal. To do this you would take their set and project one on the other and draw a line from the two projects. This forms an orthonormal set. This is called [[Gram-Schmidt Orthonormalization]].

[[Einstein Summation Convention]]: If we have a basis: $\{\ket{e_1}, ... \ket{e_n}\}$ of $V$, we can decompose each vector $\ket{v}$ into components:
$$\ket{v}=v^\mu \ket{e_\mu}$$ where: $v^\mu \in F \times F \times ... \times F = F^n$ 