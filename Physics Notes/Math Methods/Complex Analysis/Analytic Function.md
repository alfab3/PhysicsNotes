An analytic function written as:
$$\begin{equation}
    f(z) = u(x,y) + iv(x,y)
\end{equation}$$
Analytic if the Cauchy-Riemann Conditions are satisfied
$$\begin{align}
    \frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \; \frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}
\end{align}$$
Means the analytic function is not a function of the other linearly independent combinations, it is a function of the combination $x+i y$ with no reference to $x - i y$. An analytic function can be defined as:
$$\begin{equation}
    \frac{\partial f}{\partial z*} = 0 \; -> \frac{\partial f}{\partial x} - i\frac{\partial f}{\partial y} = 0
\end{equation}$$
Plugging in gives the Cauchy-Riemann conditions, as long as there is no dependence on $z*$ at all. $X$ and $Y$ are given by:
$$\begin{align}
    x = \frac{z + z*}{2}\\
    y = \frac{z - z*}{2i}
\end{align}$$
A quick way to check if a function is analytic or not is to determine if it has first-order derivatives, and then determine if it has any dependence on $z*$. Example: is $f(z) = x$ an analytic function? No, because the Cauchy-Riemann Conditions tell you, you cant have a function that is analytic in a certain region if that region has no imaginary part at all. If it is purely or purely imaginary it cannot be analytic. As shown above $x$ has a dependence on $z*$ therefore it cannot be analytic.
$$\begin{align}
    z = re^{i\theta}
\end{align}$$
Where,
$$\begin{align}
    r = \sqrt{x^2 + y^2}\\
    \theta = tan^{-1}(\frac{y}{x})
\end{align}$$
Is r an analytic function?
$$\begin{align}
    r = (z z*)^{1/2}
\end{align}$$
No it depends on $z*$. What about theta?
$$\begin{align}
    \theta = \frac{1}{2i}\ln (\frac{z}{z*})
\end{align}$$
No it also depends on $z*$. Analytic functions must follow a very specific structure. The Cauchy-Riemann conditions also tell us:
$$\begin{equation}
    \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0 = \frac{\partial^2 v}{\partial x^2} + \frac{\partial^2 v}{\partial y^2}
\end{equation}$$
In the region in which some function $f(z)$ is analytic the real part and imaginary part separately satisfy Laplace's equations. Solutions of Laplace's equations are called harmonics.

If $f(z)$ is analytic for all $|z| < \infty$ then $f(z)$ is an entire function.