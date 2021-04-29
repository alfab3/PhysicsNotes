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
