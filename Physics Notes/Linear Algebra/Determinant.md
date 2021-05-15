The determinant is the factor in which an area of space changes after undergoing a transformation([[Linear Transformations and Matrices]]). If the determinant is negative the space is actually flipped and then scaled. To calculate it numerically:
$$\begin{align}
    det
    \begin{bmatrix}
        a \; \;b\\
        c \; \;d
    \end{bmatrix}
    =
    ad - bc
\end{align}$$
If a determinant is 0, this means the transformation represented my the matrix squishes space into a smaller dimension.

Given a Linear operator L with components $L^\mu_\nu \; (i.e., \; L\ket{e_\mu} = L^\nu_\mu \ket{e}$ then the determinant of $L$ is 
$$det(L) = det(L^\nu_\mu)$$ 