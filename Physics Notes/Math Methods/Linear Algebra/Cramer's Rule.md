So let's start with a linear system of equations:
$$\begin{align}
    3x + 2y = -4\\
    x + 2y = -2
\end{align}$$
Of course this would work for larger system with equal amounts of unknowns and equations. You can think about this setup geometrically: 
$$\begin{align}
    \begin{bmatrix}
        3 \; \;2\\
        1 \; \;2
    \end{bmatrix}
    \begin{bmatrix}
        x\\
        y
    \end{bmatrix}
    =
    \begin{bmatrix}
        -4\\
        -2
    \end{bmatrix}
\end{align}$$
Where the first matrix is transforming the unknown vector and we know what the output is going to be. So the puzzle is what is the input that will give us this output? We know that the given output vector is some linear combination of the columns of the matrix. Side note - transformations that preserve dot products are called orthonormal. So to determine the $y$ coordinate of the new vector you would take the new area after the transformation([[Linear Transformations and Matrices]]) and divide it by the original area. 
$$\begin{align}
    y = \frac{Area}{det(A)} = \frac{det
    \begin{bmatrix}
        2 \; \;4\\
        0 \; \;2
    \end{bmatrix}
    }
    {det
    \begin{bmatrix}
        2 \; \;-1\\
        0 \; \;1
    \end{bmatrix}
    }
\end{align}$$
For x it would be the same:
$$\begin{align}
    x = \frac{Area}{det(A)} = \frac{det
    \begin{bmatrix}
        4 \; \;-1\\
        2 \; \;1
    \end{bmatrix}
    }
    {det
    \begin{bmatrix}
        2 \; \;-1\\
        0 \; \;1
    \end{bmatrix}
    }
\end{align}$$