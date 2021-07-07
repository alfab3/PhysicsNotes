We start with something called a Linear system of equations which look something like this:
$$\begin{align}
    2x + 5y + 3z = -3\\
    4x + 0y + 8z = 0 \\
    1x + 3y + 0z = 2
\end{align}$$
Which can be represented in the form: 
$$\begin{align}
    \begin{bmatrix}
        2 \; \; 5 \; \; 3\\
        4 \; \; 0 \; \; 8\\
        1 \; \; 3 \; \; 0
    \end{bmatrix}
    \begin{bmatrix}
        x\\
        y\\
        z
    \end{bmatrix}
    =
    \begin{bmatrix}
        -3\\
        0\\
        2
    \end{bmatrix}
\end{align}$$
This can be represented as a formula: $A\vec{x} = \vec{v}$. Where $A$ represents the matrix. You can think about this as $A$ is the transformation to move $\vec{x}$ to $\vec{v}$.
To reverse a transformation, say going from $\vec{v}$ back to $\vec{x}$ you would use the inverse matrix (transformation)([[Linear Transformations and Matrices]]). Written as:
$$\begin{align}
    A^{-1} = 
    \begin{bmatrix}
        3 \; \; 1\\
        0 \; \; 2\\
    \end{bmatrix}
    ^{-1}
\end{align}$$
If the $det(A) =/= 0$ then $A^{-1}$ exists. Another term that is important to this is "rank" where rank is the number of dimensions in the output.