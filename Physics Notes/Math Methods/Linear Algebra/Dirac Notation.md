Kets - Say you have a traditional vector in 3D space: 
$$\vec{v} = 
\begin{bmatrix}
        x\\
        y\\
		z
    \end{bmatrix}$$
With [[Basis Vectors]] in 3 Dimensional space defined generally as: 
$$\vec{e_1} = 
\begin{bmatrix}
        1\\
        0\\
		0
\end{bmatrix}$$

$$\vec{e_2} = 
\begin{bmatrix}
        0\\
        1\\
		0
\end{bmatrix}$$

$$\vec{e_i} = 
\begin{bmatrix}
        0\\
        ...\\
		1
\end{bmatrix}$$

This means any vector can be decomposed into a [[Linear Combination]] of [[Basis Vectors]]... $$\vec{v} = \sum_i v_i e_i = xe_1 + ye_y + ze_3$$

Similarly using Dirac notation, $$\vec{v} = \ket{v} = 
\begin{bmatrix}
        x\\
        y\\
		z
\end{bmatrix} $$

The [[Basis Vectors]] can also be written as kets
$$\ket{1} = 
\begin{bmatrix}
        1\\
        0\\
		0
\end{bmatrix}$$

$$\ket{2} = 
\begin{bmatrix}
        0\\
        1\\
		0
\end{bmatrix}$$

$$\ket{i} = 
\begin{bmatrix}
        0\\
        ...\\
		i
\end{bmatrix}$$

This means any vector can be decomposed into a [[Linear Combination]] of [[Basis Vectors]]... $$\vec{v} = \sum_i v_i \ket{i} = x\ket{1} + y\ket{2} + z\ket{3}$$

Bras - Let's consider the same vector in 3Dimensional space but let's take the transpose and complex conjugate of our original vector: 
$$\vec{v}^*_T = [x \; \; y \; \; z]$$
Side note - this operation is referred to as the Hermitian conjugate and is denoted with a dagger: 
$$\vec{v}^\dagger = [x \; \; y \; \; z]$$

$$\vec{v}^\dagger = \bra{v} = [x \; \; y \; \; z]$$

Brakets

