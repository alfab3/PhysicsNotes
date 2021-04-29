If you were to take a 2D space and rotate it 90 degrees then apply a shear to keep the grid lines parallel and equal distant apart, you would be applying what is called a composition of rotation and shear. So once again you record where $\hat{i}$ and $\hat{j}$ land. So in 2x2 matrix form (assuming they were initially located in the proper space)
$$\begin{align}
    \begin{bmatrix}
    1 \; -1\\
    1 \; \; 0
    \end{bmatrix}
\end{align}$$
The long way to calculate the transformation([[Linear Transformations and Matrices]]) of some vector is to first left multiply it by the rotation matrix then left multiply by the shear matrix. So you would have something like this:
$$\begin{align}
    \begin{bmatrix}
    1 \; \;1\\
    0 \; \;1
    \end{bmatrix}
    [
    \begin{bmatrix}
    0 \; \; -1\\
    1 \; \; 0
    \end{bmatrix}
    \begin{bmatrix}
    x\\
    y
    \end{bmatrix}
    ] = 
    \begin{bmatrix}
    1 \; -1\\
    1 \; \; 0
    \end{bmatrix}
    \begin{bmatrix}
    x\\
    y
    \end{bmatrix}
\end{align}$$
If we have two matrices of 2x2 (for example the rotation and the shear you would think of it as applying a transformation to a vector twice. In general form, numerically it would look like this:
$$\begin{align}
    \begin{bmatrix}
        a \; \;b\\
        c \; \;d
    \end{bmatrix}
    \begin{bmatrix}
        e \; \; f\\
        g \; \; h
    \end{bmatrix}
\end{align}$$
Where does $\hat{i}$ go? Well transform the first vector (column):
$$\begin{align}
    \begin{bmatrix}
        a \; \;b\\
        c \; \;d
    \end{bmatrix}
    \begin{bmatrix}
        e\\
        g
    \end{bmatrix}
    =
    e
    \begin{bmatrix}
        a\\
        c
    \end{bmatrix}
    + g
    \begin{bmatrix}
        b\\
        d
    \end{bmatrix}
\end{align}$$
Then we will transform the second vector (column)
$$\begin{align}
    \begin{bmatrix}
        a \; \;b\\
        c \; \;d
    \end{bmatrix}
    \begin{bmatrix}
        f\\
        h
    \end{bmatrix}
    =
    f
    \begin{bmatrix}
        a\\
        c
    \end{bmatrix}
    + h
    \begin{bmatrix}
        b\\
        d
    \end{bmatrix}
\end{align}$$

So the final form will look like: 
$$\begin{align}
    \begin{bmatrix}
        a \; \;b\\
        c \; \;d
    \end{bmatrix}
    \begin{bmatrix}
        e \; \; f\\
        g \; \; h
    \end{bmatrix}
    =
    \begin{bmatrix}
        a e + b g \; \;a f + b h\\
        c e + d g \; \; c f + d h
    \end{bmatrix}
\end{align}$$
Remember transformation(multiplication) order matters.

If we had the elements of the linear vector space: $\phi,\psi,....$ we would like to associate with each vector a scalar:
$$\begin{align}
    (\phi, \psi) = S_{\phi}[\psi]
\end{align}$$
Which is a scalar that depends on special element $\phi$ and is dependent on $\psi$. For every element of this vector space we choose a special element $\phi$ where something is done with the special element $\psi$ and we get a scalar function. With a certain number of properties. Those properties are:
$$\begin{align}
    (\phi,a\psi) = a(\phi,\psi)\\
    (\phi, \psi + \chi) = (\phi, \psi) + (\phi, \chi)
\end{align}$$
For every element with these properties, you can find a scalar. The set of all the scalars form a linear vector space. The set of linear functionals $\{S_{\chi}[\psi],...\}$ is a [[Linear Vector Spaces]], the [[dual]] $\tilde{V}$ of $V$. So [[linear vector spaces]] come in pairs.

What is the use of this? There is a natural way to associate a scalar with a vector which is called the [[dot product]]. It is a bi-linear operation. The vector space $(\phi,\psi) = \{S_{\phi}[\psi]\}$ which consists of the set of elements shown before, is represented by $\ket{\psi} \in V$, and the $\phi$ is represented by $\bra{\phi}$, which is a different kind of vector which lives in the "[[dual]]" space.  So if we have $(\phi, \psi)$ this is written as $\braket{\phi|\psi}$
$$\begin{align}
    \begin{bmatrix}
    x_1\\
    x_2\\
    \vdots \\
    x_n
    \end{bmatrix}
    \in \mathbb{R}^n
\end{align}$$
If we construct the corresponding row vector, all the row vectors are elements of the [[dual]] of the column vector.
$$\begin{align}
    (x_1, x_2, ..., x_n) \in \tilde{\mathbb{R}}^n
\end{align}$$
To produce a scalar that satisfies the properties, which is matrix multiplication, with the bra vector on the left and the ket vector on the right, or the row vector on the left and the column vector on the right. 
$$\begin{align}
    (x_1, x_2, ..., x_n)
    \begin{bmatrix}
    y_1\\
    y_2\\
    \vdots \\
    y_n
    \end{bmatrix}
    = x_1 y_1 +...+ x_n y_n
\end{align}$$
$\bra{\psi}\ket{\phi}$ - scalar product or inner product, we can also define this: $\bra{\psi}\ket{\psi}$. Well it can be written as:
$$\begin{align}
    (x_1, x_2, ..., x_n)
    \begin{bmatrix}
    x_1\\
    x_2\\
    \vdots \\
    x_n
    \end{bmatrix}
    = \sum_{i=1}^n x_i^2
\end{align}$$
Which is the square of the length of this vector. What if the quantities were multiplied by complex numbers? How would we preserve the properties? We would  define the element in dual space by taking the complex conjugate. So if our matrices were made of elements from some generalized vector space:
$$\begin{align}
    (\alpha_1^*, \alpha_2^*, ..., \alpha_n^*)
    \begin{bmatrix}
    \alpha_1\\
    \alpha_2\\
    \vdots \\
    \alpha_n
    \end{bmatrix}
    = \sum_{i=1}^n |\alpha_i|^2
\end{align}$$
Where the column corresponds to $\ket{\psi}$ and the row corresponds to $\bra{\psi}$ if a $\ket{\psi} = \ket{\psi '}$ then $\bra{\psi '} = a^*\bra{\psi}$. This also shows that (in complex space):
$$\begin{equation}
    \bra{\phi}\ket{\psi}^* = \bra{\psi}\ket{\phi}
\end{equation}$$