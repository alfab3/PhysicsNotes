Laplace's Equations is a second-order partial differential equation. Written as:
$$\begin{align}
    \nabla ^2f = 0 \\
    \Delta f = 0
\end{align}$$
In different coordinate systems it takes the forms:\\
Rectangular coordinates: 
$$\begin{equation}
    \nabla ^2 f = \frac{\partial ^2 f}{\partial x^2} + \frac{\partial ^2 f}{\partial y^2} + \frac{\partial ^2 f}{\partial z ^2} = 0
\end{equation}$$
Cylindrical Coordinates:
$$\begin{equation}
    \nabla ^2 f = \frac{1}{r} \frac{\partial}{\partial r} (r\frac{\partial f}{\partial r})+\frac{1}{r^2}\frac{\partial^2 f}{\partial \phi^2} + \frac{\partial ^2 f}{\partial z^2} = 0
\end{equation}$$
Spherical Coordinates:
$$\begin{equation}
    \nabla ^2 f = = \frac{1}{r^2} \frac{\partial}{\partial r}(r^2 \frac{\partial f}{\partial r}) + \frac{1}{r^2 sin \theta}\frac{\partial}{\partial \theta}(sin\theta \frac{\partial f}{\partial \theta}) + \frac{1}{r^2 sin^2 \theta} \frac{\partial ^2 f}{\partial \phi^2} = 0
\end{equation}$$

In rectangular coordinates the Laplace equation has the form:
$$\begin{equation}
    \frac{\partial ^2 \psi}{\partial x^2} + \frac{\partial ^2 \psi}{\partial y^2} = \psi_{xx} + \psi_{y y} = 0
\end{equation}$$
The real and imaginary parts of a complex analytic function both satisfy the Laplace equation. That is if $z = x + i y$ and if  $f(z) = u(x,y) + i v(x,y)$. For $f(z)$ to be analytic $u$ and $v$ must be differentiable and the Cauchy-Riemann equations be satisfied: $u_x = v_y$, $v_x = -u_y$.Given a harmonic function, it is the real part of an analytic function. If a trial form is: $f(z) = \phi(x,y) + i\psi(x,y)$ then the Cauchy-Riemann equations will be satisfied if we set: $\psi_x = - \phi_y$,$\psi_y = \phi_x$/ This relation does not determine $\psi$ but only its increments $d\psi = -\phi_y d x + \phi_x d y$. The Laplace equation for $\phi$ implies that the integrability condition for $\psi$ is satisfied: $\psi_{x y} = \psi_{y x}$. The resulting pair of solutions of the Laplace equation are called conjugate harmonic functions.