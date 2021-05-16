In variational problems we are provided with an expression $J[y]$ that "eats" whole functions $y(x)$ and returns a single number. Such objects are called functionals to distinguish them from ordinary functions. An ordinary function is a map $f:\mathbb{R} \rightarrow \mathbb{R}$. A functional $J$ is a map $J:C^\infty(\mathbb{R}) \rightarrow \mathbb{R}$ where $C^\infty(\mathbb{R})$ is the space of smooth (having derivatives of all orders) functions. To find the function $y(x)$ that maximizes or minimizes a given functional $J[y]$ we beed to define and evaluate, its [[Functional Derivative]]

The functional assigns a real value to one or more functions of the given class. 
$$
F[f] = \int^{x_b}_{x_a} g(f, f_x, x)dx
$$
Here $f$ is a differentiable function, $x$ is the argument of the function $f$, $f_x \equiv f'(x)$ is the derivative of the function f, and g is a certain fixed differentiable function of three variables.
Apart from being differentiablem the function $f(x)$ is typically subject to certain constraints. For example 
$$
f(x_a) = y_a
$$
with $y_a$ certain fixed numbers. 
Example: 
Length of a line in a plane:


Functional of many functions
The generalization of the theory to the case of more than one function, $f \rightarrow f^{(1)}, f^{(2)},...,f^{(m)}$ is quite straightforward. Now we have 
$$
F[f^{(1)}, f^{(2)},...,f^{(m)}] = \int^{x_b}_{x_a} g(f^{(1)}, f^{(2)},...,f^{(m)},f_x^{(1)}, f_x^{(2)},...,f_x^{(m)}, x)dx
$$
$$
f^{(j)}(x_a) = y_a^{(j)}, \;\; f^{(j)}(x_b) = y_b^{(j)}, \;\; (j = 1,2,...,m)
$$
Introducing the variations 
$$
f^{(j)} \rightarrow f^{(j)} + \delta f^{(j)}
$$
and evaluating $\delta F$
$$
\delta F = \sum^m_{j=1} \int^{x_b}_{x_a} A_j(x) \delta f(j)xdx
$$
$$
A_j(x) = \frac{\partial g}{\partial f^{(j)}}-\frac{d}{dx}\frac{\partial g}{\partial f_x^{(j)}}
