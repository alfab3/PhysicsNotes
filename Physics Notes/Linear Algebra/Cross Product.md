Imagine you have two vectors, $\vec{v}$ and $\vec{w}$ if you look at them in 2D they form a parallelogram. Different orientation of the [[Vectors]] and how they are written in the formula will affect the sign of the cross product. To calculate the cross product you place both vectors as the columns of a 2 x 2 matrix and then compute the determinant of that new matrix. So the parallelograms area is the length of the new vector, while the direction is perpendicular to the other vectors you can use the right hand rule to find out the direction. To use the [[Determinant]]method to calculate the cross product you use:
$$\begin{align}
    \begin{bmatrix}
        v_1\\
        v_2\\
        v_3
    \end{bmatrix}
    \times
    \begin{bmatrix}
        w_1\\
        w_2\\
        w_3
    \end{bmatrix}
    =
    det
    \begin{bmatrix}
        \hat{i} \; \; v_1 \; \;w_1\\
        \hat{j} \; \; v_2 \; \;w_2\\
        \hat{k} \; \; v_3 \; \;w_3
    \end{bmatrix}
\end{align}$$