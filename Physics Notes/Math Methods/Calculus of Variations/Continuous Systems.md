Suppose we are given an action functional $S[\phi]$ depending on a field $\phi(x^\mu)$ and its first derivatives

$$
\phi_\mu \equiv \frac{\partial \phi}{\partial x^\mu}
$$
Here $x^\mu$, $\mu = 0,1,...,d$, are the coordinats of a $(d+1)$-dimensional space-time. It is traditional to take $x^0 \equiv t$ and the other coordinates space-like. Suppose further that 
$$
S[\phi] = \int L dt = \int \mathcal{L}(x^\mu, \phi, \phi_\mu)d^{d+1}x,
$$
where $L$ is the [[Lagrangian Density]], in terms of which 
$$
L = \int \mathcal{L}d^dx
$$
and the integral is over the space coordinates. Now 
$$\begin{gather}
\delta S = \int \{\delta \phi(x) \frac{\partial \mathcal{L}}{\partial \phi (x)} + \delta(\phi_\mu(x)) \frac{\partial \mathcal{L}}{\partial \phi_\mu (x)} \}d^{d+1}x = 
\end{gather}$$
$$\begin{gather}
\int \delta \phi(x) \{\frac{\partial \mathcal{L}}{\partial \phi (x)} -\frac{\partial}{\partial x^\mu} \frac{\partial \mathcal{L}}{\partial \phi_\mu (x)} \}d^{d+1}x
\end{gather}$$
In going from the first to the second, we observe that 
$$
\delta(\phi_\mu(x)) = \frac{\partial}{\partial x^\mu}
$$
and used the [[Divergence Theorem]], 
$$
\int_\Omega \frac{\partial A^\mu }{\partial x^\mu}d^{n+1}x = \int_{\partial \Omega} A^\mu n_\mu DS.
$$
The result is that 
$$
\frac{\delta S}{\delta \phi(x)} = \frac{\partial \mathcal{L}}{\partial\phi(x)} - \frac{\partial}{\partial x^\mu}(\frac{\partial \mathcal{L}}{\partial \phi_\mu}(x))
$$
and the equation of motion comes from setting this to zero. 