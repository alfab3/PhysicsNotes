Let's consider the second-order self-adjoint inhomogeneous ODE
$$
\mathcal{L}y \equiv \frac{d}{dx}\bigg(p(x)\frac{dy}{dx}\bigg) + q(x)y = f(x)
$$
which is to be satisfied on the range $a \leq x \leq b$ subject to homogeneous boundary conditions at $x=a$ and $x=b$. Our Green's Function for this problem needs to satisfy the boundary conditions and the [[Ordinary Differential Equation]] 
$$\begin{align} \mathcal{L}G(x,t) = \delta(x-t) \end{align}$$
so that $y(x)$, the solution to the initial equation  with its boundary conditions, can be obtained as 
$$\begin{align} y(x) = \int^b_aG(x,t)f(t)dt \end{align}$$
To verify this equation sinply apply $\mathcal{L}$:
$$\begin{align} \mathcal{L}y(x) = \int_a^b \mathcal{L} G(x,t) f(t) dt = \int^b_a \delta(x -t) f(t) d(t) \end{align} = f(x)$$