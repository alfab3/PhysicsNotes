In linear algebra we think of coordinates as something that scales a vector in our case this would be the basis vectors. There are some implicit assumptions using these two basis vectors:
1) The First Coordinate indicates rightward motion
2) tem The second coordinate indicates upward motion
3) Unit of distance
What if we used different basis vectors? For example, what if we used the set of [[Basis Vectors]]: $\vec{b_1}$ and $\vec{b_2}$. In the original basis if we had a vector say: 
$$\begin{align}
    \begin{bmatrix}
        3\\
        2
    \end{bmatrix}
\end{align}$$
Which can also be written as $3\hat{i} + 2\hat{j}$. In the other basis this vector would actually be described as:
$$\begin{align}
    \begin{bmatrix}
        5/3\\
        1/3
    \end{bmatrix}
\end{align}$$
Which can be written in the other basis as: $(5/3)\vec{b_1}+(1/3)\vec{b_2}$. The [[Basis Vectors]] in the alternative basis can be though of in our basis as:
$$\begin{align}
    \vec{b_1} \rightarrow
    \begin{bmatrix}
        2\\
        1
    \end{bmatrix}
    ,
    \vec{b_2} \rightarrow
    \begin{bmatrix}
        -1\\
        1
    \end{bmatrix}
\end{align}$$
But in the alternative basis they are thought of as: 
$$\begin{align}
    \vec{b_1} \rightarrow
    \begin{bmatrix}
        1\\
        0
    \end{bmatrix}
    ,
    \vec{b_2} \rightarrow
    \begin{bmatrix}
        0\\
        1
    \end{bmatrix}
\end{align}$$
The origin will always line up. 
How do we translate between coordinate systems? If a vector in the alternative coordinate system is described as: $-1\vec{b_1}+2\vec{b_2}$ what would that be in our coordinate system? From out perspective, the alternative [[Basis Vectors]] are described as written in eq. 1.33. So we can compute: 
$$\begin{align}
    \begin{bmatrix}
        ?\\
        ?
    \end{bmatrix}
    =
    -1
    \begin{bmatrix}
        2\\
        1
    \end{bmatrix}
    +2
    \begin{bmatrix}
        -1\\
        1
    \end{bmatrix}
    =
    \begin{bmatrix}
        -4\\
        1
    \end{bmatrix}
\end{align}$$
So in the original basis the vector $-1\vec{b_1}+2\vec{b_2}$ would be described as $-4\hat{i}+1\hat{j}$. This shows that the way to transform from the alternative basis to the original, you would do matrix multiplication where the transformation matrix consists of columns of the [[Basis Vectors]] of the alternative basis in out basis: 
$$\begin{align}
    \begin{bmatrix}
        2\;\;-1\\
        1\;\;1
    \end{bmatrix}
    \begin{bmatrix}
        -1\\
        2
    \end{bmatrix}
    = -1
    \begin{bmatrix}
        2\\
        1
    \end{bmatrix}
    +2
    \begin{bmatrix}
        -1\\
        1
    \end{bmatrix}
    =
    \begin{bmatrix}
        -4\\
        1
    \end{bmatrix}
\end{align}$$
To convert to the original basis to the new basis: you take the inverse ([[Inverse Matrices]]) of the transformation matrix ([[Linear Transformations and Matrices]])
$$\begin{align}
    \begin{bmatrix}
        2\;\;-1\\
        1\;\;1
    \end{bmatrix}
    ^{-1}
    =
    \begin{bmatrix}
        1/3 \; \; 1/3\\
        -1/3 \; \; 2/3 
    \end{bmatrix}
\end{align}$$
In General: 
$$\begin{align}
    A
    \begin{bmatrix}
        x_j\\
        y_j
    \end{bmatrix}
    =
    \begin{bmatrix}
        x_0\\
        y_0 
    \end{bmatrix}
\end{align}$$
Where $A$ is the alternative basis vectors written in our coordinates and 
$$\begin{align}
    \begin{bmatrix}
        x_j\\
        y_j
    \end{bmatrix}
\end{align}$$
Describes a vector in the alternative coordinate system and
$$\begin{align}
    \begin{bmatrix}
        x_0\\
        y_0
    \end{bmatrix}
\end{align}$$
Describes a vector in the original coordinate system. Therefore to do the reverse: 
$$\begin{align}
    \begin{bmatrix}
        x_j\\
        y_j
    \end{bmatrix}
    =
    A^{-1}
    \begin{bmatrix}
        x_0\\
        y_0 
    \end{bmatrix}
\end{align}$$