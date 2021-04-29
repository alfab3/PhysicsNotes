Definition: A Subspace of the vector space [[Linear Vector Spaces]] $V$ is a subset $W \subseteq V$ that is also a vector under the same operations.

Theorem: $W \subseteq V$ is a subspace if and only if 
1) $\ket{0} \in W$
2) $W$ is closed under t

Subspace of $\mathbb{R}^n$ 
A subset of vectors $V$ of $\mathbb{R}^n$. $V$ is a subspace of $\mathbb{R}^n$ if:
1) $V$ contains the $0$
2) $\vec{x}$ in $V$ $c\vec{x}$ is in $V$ - closure under scalar multiplication which means if you multiply the vector by a real scalar the result should be within the subspace otherwise $V$ is not a subspace. 
3) If there are two vectors in the subspace say $\vec{a} \in V$ and $\vec{b} \in V$ then $\vec{a} + \vec{b} \in V$ - closure under addition 

Example: Say we have some subset: 
$$S = \{
\begin{bmatrix}
	x_1\\
	x_2
\end{bmatrix}
\in \mathbb{R}^2 | x_1 \geq 0\}$$
is $S$ a subspace of $\mathbb{R}^2$?
1) Does it contain the zero vector: Yes
2) Closed under addition: 

$$\begin{bmatrix}
	a\\
	b
\end{bmatrix}
+
\begin{bmatrix}
	c\\
	d
\end{bmatrix}
=
\begin{bmatrix}
	a + b\\
	b + d
\end{bmatrix}$$

3) Closed under multiplication:

$$
-1
\begin{bmatrix}
	a\\
	b
\end{bmatrix}
=
\begin{bmatrix}
	-a\\
	-b
\end{bmatrix}
$$

This subset is not a subspace of $\mathbb{R}^2$ because it is not closed under scalar multiplication.