[[Functional]]
The functional assigns a real value to one or more functions of the given class. 
$$\begin{align}
F[f] = \int^{x_b}_{x_a} g(f, f_x, x)dx
\end{align}$$
Here $f$ is a differentiable function, $x$ is the argument of the function $f$, $f_x \equiv f'(x)$ is the derivative of the function f, and g is a certain fixed differentiable function of three variables.
Apart from being differentiablem the function $f(x)$ is typically subject to certain constraints. For example 
$$\begin{align}
f(x_a) = y_a
\end{align}$$
with $y_a$ certain fixed numbers. 

[[Euler's Equation]]
The condition that the integral of a [[Functional]] has an extremum requires a formula such that the Functional has a maximum or minimum value.

Assume we are looking for some function $y(x)$ such that the integral:

$$\begin{align} J = \int^{x_b}_{x_a}f\{y(x),\ y'(x);\ x\} dx\end{align}$$

is an extremum (min or max).The points $x_a$ and $x_b$ are fixed.

Then we use: 
$$\begin{align} \frac{\partial f}{\partial y} - \frac{d}{dx}\frac{\partial f}{\partial y'} = 0\end{align}$$

