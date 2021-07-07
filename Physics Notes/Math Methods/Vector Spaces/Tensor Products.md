Given two vector spaces ([[Linear Vector Spaces]]) $V$ and $W$, the tensor product $V \otimes W$ is defined as follows: 

1) $\forall \ket{v}  \in V, \ket{w} \in W$ a decomposable element of $V \otimes W$ is the vector $$ \ket{v} \otimes \ket{w} $$ not all elements of $V \otimes W$ are decomposable
2) The tensor product is bilinear, i.e., $$(\ket{v_1}+\lambda\ket{v_2}) \otimes \ket{w} = \ket{v_1} \otimes \ket{w} + \lambda\ket{v_2} \otimes \ket{w}\ket{v} \otimes (\ket{w_1} + \lambda\ket{w_2}) = \ket{v}\otimes\ket{w_1} + \lambda\ket{v} \otimes \ket{w_2}$$
3) the full tensor product space is the [[Span]] of it decomposable elements: $$V \otimes W = span\{\ket{v} \otimes \ket{w} | \ket{v}\in V, \ket{w} \in W \}$$

The last property allows to construct a [[Basis Set]] of $V \times W$ as follows:
if $\{\ket{e_1},...,\ket{e_n}\}$ is a basis of $V$ and $\{\ket{e_1'},...,\ket{e_m'}\}$ is a basis of $W$ then 
$$\{\ket{e_1} \otimes \ket{e_1'}, \ket{e_1} \otimes \ket{e_2'},...,\ket{e_1}\otimes\ket{e'_m}, \ket{e_2} \otimes \ket{e_1'}, \ket{e_2} \otimes \ket{e_2'},..., \ket{e_2} \otimes \ket{e_m'},..., \ket{e_n} \otimes \ket{e_1'}, \ket{e_n} \otimes \ket{e_2'},... \ket{e_n} \otimes \ket{e_m'} \}$$ is a basis of $V \otimes W$

It follows that $dim(U \otimes V) = (dim(U))(dim(V))$ also $F \otimes V \simeq V$ (F is 1-dimensional) $\{\ket{0}\} \otimes V \simeq \{\ket{0}\}(\ket{0} is 0-dimensional$ 

Simple example: if $V = \mathbb{R}^7, W = \mathbb{R}^3$ then $V \otimes W$ is the set of the $2 \times 3$ matrices, and the decomposable elements of $V \otimes W$ 

$$\begin{bmatrix}
	v_1w_1 \; \; v_1w_2 \; \; v_1w_3 \\
	v_2w_1 \; \; v_2w_2 \; \; v_2w_3
\end{bmatrix}$$

where $v_1,v_2; w_1, w_2, w_3$ are reals
