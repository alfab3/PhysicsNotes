Potential energy of a flexible cable suspended from two fixed points.

y - axis is perpendicular to the surface of the earth

the cable is represented by a curve: $y=f(x)$ in the $xy$ plane, with constraint: $$\begin{align}f(x_a) = y_a, \;\; f(x_b)=y_b\end{align}$$

The potential energy of the element $dl$ is proportional to its height $y$ and its length $dl$

Hence the total potential energy is given by the integral
$$\begin{align} U[f] = \int ydl = \int^{x_b}_{x_a} f\sqrt{1+y'^2}\ dx\end{align}$$

$U[f]$ has the form:

$$\begin{align} g(y,\ y',\ x) = f\sqrt{1+y'^2}\end{align}$$

To use [[Lagrange Multipliers]] we write a new [[Functional]]:
$$\begin{align}\tilde{F} = F[f] -\lambda Q[f] \end{align}$$

Hence:

$$\begin{align} \tilde{F}[y] = \int^{x_b}_{x_a}[g(y,\ y'; \ x)-\lambda q(y,y'; x)\;dx] = \int^{x_b}_{x_a}(f-\lambda)\sqrt{1+(y')^2}\end{align}$$

Now introduce the new function $$\begin{align} \tilde{y} = y - \lambda \end{align}$$

in which case we get:

$$\begin{align} \tilde{F}[\tilde{y}] = \int^{x_b}_{x_a} \tilde{y}\sqrt{1+(\tilde{y'})^2}\;dx\end{align}$$