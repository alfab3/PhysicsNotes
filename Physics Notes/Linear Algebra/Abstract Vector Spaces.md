Geometrically, going to higher dimensions are hard to conceptualize. However, computationally performing linear algebra actually shows that the math is not reliant on the underlying coordinate system, the coordinates are actually arbitrary. [[Determinant]]s and [[Eigenvectors]] are indifferent over coordinate systems. So let's look at something with vector properties: functions. Functions, in a sense, are actually just another type of vector. For example you can add two functions together, like two vectors. Say we have two functions $f(x)$ and $g(x)$ you can add them together: $(f+g)$ which is a new function. The output of this new function at any given input say $-4$, is the sum of the outputs $f$ and $g$: $(f+g)(-4.00) = f(-4.00) + g(-4.00)$, when you evaluate them each at that same input $-4.00$. More generally: 
$$\begin{align}
    (f+g)(x) = f(g)+g(x)
\end{align}$$
This is similar to adding [[Vectors]] coordinate by coordinate. You can also scale a function by a real number:
$$\begin{align}
    (2f)(x) = 2f(x)
\end{align}$$
Which is just scaling the output, this is similar to scaling a vector coordinate by coordinate, even though there are infinitely many coordinates. While [[Vectors]]really can only be added together or scaled. We may be able to take the other problem solving constructs originally for vectors and apply them to functions. For example a linear transformation, which can take an a function as an input and output another. Formal definition of Linearity: 
$$\begin{align}
    Additivity: \; \; L(\vec{v}+\vec{w}) = L(\vec{v}+\vec{w})\\
    Scaling: \; \; L(c\vec{v}) = c L(\vec{v})
\end{align}$$
An example of this for functions is the derivative. The derivative of a function is linear:
$$\begin{align}
    \frac{d}{d x}(x^3+x^2) = \frac{d}{d x}(x^3) + \frac{d}{d x}(x^2)\\
    \frac{d}{d x}(4x^3) = 4\frac{d}{d x}(x^3)
\end{align}$$
To see this parallel, let's describe the derivative with a matrix. We must first give coordinates to this space which requires choosing a basis. Since polynomials are already written down as the sum of scaled powers of the variable $x$ we can construct basis functions from the pure powers of x.
$$\begin{align*}
    b_0(x) = 1\\
    b_1(x) = x\\
    b_2(x) = x^2\\
    b_3(x) = x^3\\
    \vdots
\end{align*}$$
The roles of these basis functions is similar to the role of $\hat{i}$, $\hat{j}$, and $\hat{k}$. Since our set of polynomials can have infinitely many degrees our set of basis functions is infinite.