An inner product on a vector space  [[Linear Vector Spaces]] $V$ is a function $\braket{., .}: V \times V \rightarrow F$ such that
1) $\braket{v|w} + \lambda \ket{x}> = \braket{v|w} + \lambda \braket{v|x}$
2) $\braket{v|w} = \braket{w|v}^*$
3) $<\braket{x|x}> \geq 0$ and $<\braket{x|x}> = 0$ 

Example: given two column vectors if $\mathbb{c}^2$:

$$\begin{bmatrix}
	a \\
	b
\end{bmatrix}
,
\begin{bmatrix}
	x \\
	y
\end{bmatrix}
$$ 
the operator
$$<
\begin{bmatrix}
	a \\
	b
\end{bmatrix}
,
\begin{bmatrix}
	x \\
	y
\end{bmatrix}
>
= a^*x + b^*y$$
is an inner product.

Given an inner product $\braket{.,.}$ one can define an operator $\dagger:V \rightarrow V^*$ so that $\ket{x}^\dagger$ is a linear operator acting on $V$ through 
$$\ket{x}^\dagger (\ket{v}) = \braket{x|v}$$ 

This called the [[Hermitian Adjoint]]
So this maps a vector $\ket{x}$ to a linear operator on vectors, i.e. a covector. This 