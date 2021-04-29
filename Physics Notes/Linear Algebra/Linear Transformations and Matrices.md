If a transformation takes some input vector to some output vector, we imagine that input vector "moving" to the output vector. A linear transformation has two properties, all lines must remain lines without getting curved and the origin must remain fixed in place. Grid lines remain parallel and evenly spaced. To perform these transformations you only need to record where the two basis [[vectors]] (in our case $\hat{i}$ and $\hat{j}$) land. For example, imagine the vector:
$$\begin{align}
    \vec{v} = 
    \begin{bmatrix}
    -1\\
    2
    \end{bmatrix}
\end{align}$$
Which can also be written as $\vec{v} = -1\hat{i}+2\hat{j}$. Once this is transformed the formula looks like:
$$\begin{equation}
    Transformed \; \vec{v} = -1(Transformed \; \hat{i}) + 2(Transformed \; \hat{j})
\end{equation}$$
It ends up as the same [[linear combination]] it started with before the transformation. Which means you can deduce where $\vec{v}$ must go based on where $\hat{i}$ and $\hat{j}$ will land. In the transformed plane, the [[basis vectors]] $\hat{i}$ and $\hat{j}$ end up at $[1, -2]$ and $[3,0]$ respectively. Which means the new transformed final vector has the equation:
$$\begin{align}
    -1\begin{bmatrix}
    1\\
    -2
    \end{bmatrix}
    + 2
    \begin{bmatrix}
    3\\
    0
    \end{bmatrix}
    =
    \begin{bmatrix}
    5\\
    2
    \end{bmatrix}
\end{align}$$
This can be written in a 2 x 2 matrix form where the left column represents the $\hat{i}$ transformation and the right column represents the $\hat{j}$ transformation:
$$\begin{align}
    \begin{bmatrix}
    a \; \;
    b\\
    c \; \;
    d
    \end{bmatrix}
\end{align}$$
If we apply this transformation to some vector
$$\begin{align}
    \begin{bmatrix}
    x\\
    y
    \end{bmatrix}
\end{align}$$
Which gives us:
$$\begin{align}
    x
    \begin{bmatrix}
    a\\
    c
    \end{bmatrix}
    + y
    \begin{bmatrix}
    b\\
    d
    \end{bmatrix}
    =
    \begin{bmatrix}
    ax + by\\
    cx + dy
    \end{bmatrix}
\end{align}$$