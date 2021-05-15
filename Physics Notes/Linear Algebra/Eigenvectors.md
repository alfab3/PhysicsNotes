Consider some linear transformation in 2D that moves the [[basis vectors]] $\hat{i}$ a and $\hat{j}$ to:
$$\begin{align}
    \begin{bmatrix}
        3\\
        0
    \end{bmatrix}
    ,
    \begin{bmatrix}
        1\\
        2
    \end{bmatrix}
\end{align}$$
If we look at one particular vector when then transformation ([[Linear Transformations and Matrices]])occurs the vector gets knocked off the span. Some special vectors remain on their [[span]], they just get stretched or squished. In this special case the $x$ component of the vector [[span]]s the x-axis. So the two [[vectors]] that exhibit this property are [[vectors]] along the x,y = -1 diagonal and the line x = 0. These special vectors are called the [[eigenvectors]] of the transformation, and each have associated with it whats called an eigenvalue. Which is just the factor by which it is stretched or squished to remain on the span. [[Eigenvalues]] can be positive or negative. 
So the original way to do these transformations is to think where each basis vector lands once the transformation is applied. A better way to do this is to find the eigenvectors and eigenvalues. Symbolically here is what an eigenvector looks like:
$$\begin{align}
    A \vec{v} = \lambda \vec{v}
\end{align}$$
Where $A$ is the transformation matrix, and $\vec{v}$ is the eigenvector([[Eigenvectors]]), and $\lambda$ is the corresponding eigenvalue([[Eigenvalues]]). What this means conceptually is that the Matrix vector multiplication gives the same answer as the scalar multiplication of the eigenvalue and eigenvector. 
Scaling by $\lambda$ = [[matrix multiplication]]:
$$\begin{align}
    \begin{bmatrix}
        \lambda \; \; 0 \; \; 0\\
        0 \; \; \lambda \; \; 0 \\
        0 \; \; 0 \; \; \lambda
    \end{bmatrix}
\end{align}$$
Which can allow you to factor out $\lambda$ and you get: 
$$\begin{align}
    A\vec{v} = (\lambda I)\vec{v}
\end{align}$$
Where $I$ is the identity matrix. This allows us to rewrite:
$$\begin{align}
    (A-\lambda I)\vec{v} = \vec{0}
\end{align}$$
We want a nonzero $\vec{v}$. We need:
$$\begin{align}
    det(A-\lambda I) = 0
\end{align}$$
Because when the [[determinant]] is equal to zero we know the transformation squishes into a smaller dimension. There are cases when there are no eigenvectors, such as in cases of rotation. A rotation would cause the [[eigenvalues]] to become complex. 

$\ket{x}$ is an eigenvector of a linear operator L if there is a $\lambda \in F$, such that $L\ket{x} = \lambda\ket{x}$. $\lambda$ is called the associated eigenvalue. Then it is possible to show that if $\lambda$ is an [[Eigenvalues]] of $L$,
then 
$$det(L-\lambda \mathbb{I}) = 0$$

Now if the space has dimentsion n, then:
$$P_n(\lambda) = det(L - \lambda\mathbb{I})$$ 
is a polynomial of degree n, called the characteristic polynomial. Since every polynomial can be factored over $\mathbb{c}$ there will be n complex numbers $\lambda_1,...,\lambda_n$, such that 

>$$P_n(\lambda) = (-1)^n \Pi^n_{i=1}(\lambda-\lambda_i)$$

So that the $\lambda_i$s are the [[eigenvalues]] of $L$.

Now it is possible to show that the [[Eigenvalues]] of $L$ are the roots of the [[Minimal Polynomial]].

This implies that $P_k(\lambda)$ and $P_n(\lambda)$ have the same roots. But the two polynomial in general are of different order, to the multiplicities might be different. 

For instance one might have
$$P_k(\lambda) = \lambda^2(\lambda+1)(\lambda-2)$$
and
$$P_n(\lambda) = \lambda^3(\lambda+1)^2(\lambda-2)$$

Theorem: $L$ is [[Diagonalizable]]  $L's$ [[Minimal Polynomial]] has no multiple roots. 

The Spectral Theorem: 
All self-[[Adjoint]] operators $L$ have an orthonormal basis ([[Basis Set]]) of eigenvectors with real [[Eigenvalues]]. In other words there is an orthonormal basis $\{\ket{e_1},...,\ket{e_n}$

$$L = \sum^n_{i=1} \lambda_i \ket{e_i}\bra{e_i}$$ 

Proof to show that $L$ is [[Diagonalizable]] 
First, from $L=L^\dagger$ it follows that [[Eigenvalues]] are real. In fact from 

$$L\ket{x} = \lambda{x} = \lambda \braket{x|x} = \braket{x|L|x} = \braket{x|L^\dagger|x}^* = \braket{x|L|x}^* = \lambda^* \braket{x|x} $$
$$\lambda = \lambda^*$$

Assume the [[Minimal Polynomial]] has now a repeated root $\lambda_0$: 
$$P_k(\lambda) = (\lambda - \lambda_0)^2 P_{k-2} (\lambda)$$

then $\lambda_0$ must be real.

Also, $(L - \lambda_0 \mathbb{I})^2 P_{k-2}(L) = 0$, so that $\forall \ket{x} \in V$, 

$$\braket{x| P_{k-2}(L)^\dagger[(L-\lambda_0 \mathbb{I})^2 P_{k-2}(L)]|x} = 0$$

$$\braket{x| P_{k-2}(L)^\dagger(L-\lambda_0 \mathbb{I})^\dagger (L-\lambda_0 \mathbb{I}) P_{k-2}(L)|x} = 0$$ 

which impies $(L - \lambda_0 \mathbb{I}) P_{k-2}(L)\ket{x} = 0$ $\forall \ket{x}$

so that $(\lambda - \lambda_0)P_{k-2}(\lambda)$ is a new [[Minimal Polynomial]], in contradiction with our assumption. This proves that $L's$ minimal polynomial has only single roots and so $L$ is [[Diagonalizable]].

Finally let us prove that $L$ has an orthonormal basis of eigenvectors. To do so is enough to prove orthogonality as normalization is straightforward. Let $\ket{x}, \lambda_x, and \ket{y}, \lambda_y$ be two eigenvectors with their corresponding eigenvalue. 

Then 
$$\braket{y|L|x} = \bra{y}(L\ket{x}) = \lambda_x \braket{y|x}$$

$$(L^\dagger) \ket{y})^\dagger \ket{x} = (L\ket{y})^\dagger \ket{x} = \lambda_y \braket{y|x}$$

so that $\lambda_x - \lambda_y \braket{x|y} = 0$ eigenvectors corresponding to different eigenvalues are orthogonal. 

For [[Eigenvalues]] corresponding to multiple eigenvectors, finally one can use the [[Gram-Schmidt Orthonormalization]] procedure for the corresponding [[Subspace]]. 