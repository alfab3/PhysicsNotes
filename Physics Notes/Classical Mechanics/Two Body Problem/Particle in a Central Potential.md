We have reduced a problem of two particles to a single-particle problem with an external central potential, $U(\vec{r}) \equiv U(r)$. Let is explore the general properties of the motion in such a potential. As is easily seen, the momentum of particle is not conserved. Meanwhile, the energy,

$$
E = \frac{mv^2}{2}+U(r)
$$

and the [[Angular Momentum]] with respect to the center (origin of the coordinates)

$$
L = m\vec{r} \times \vec{v}
$$
are conserved

Conservation of the angular momentum implies one very important property of the motion in a central potential. By definition (13), we have 
$$
\vec{r} \cdot \vec{L} = 0
$$
In combination with the conservation of $L$, this means that there exists such a constant vector that at any time $t$ we have:
$$
r(t)\perp \vec{L}
$$
Hence the motion is two-dimensional: The z-component of the radius-vector is identically equal to zero if the z axis is chosen parallel to $L$. 
The combination of the two-dimensional character of the motion and the fact that $U$ depends only on the absolute value of the radius-vector suggests that we switch to [[Polar Coordinates]] $r$ and $\theta$ on the $xy$ plane
$$\begin{align}
	x = r\cos\theta \\
	y = r\sin\theta
\end{align} 
$$
In polar coordinates, the law of conservation of the angular momentum reads
$$\begin{align}
	\dot{\theta} = \frac{l}{mr^2} \; \; \; \;
	(l = |\vec{L}|=const)
\end{align}
$$
From the [[Angular Momentum]] equation we see that the angular velocity $\dot{\theta}$ does not change its sign, so that the particle permanently rotates around the center in one and the same direction, dependings on the the initial condition. We also see that the case $l = 0$ is special: Here $\theta = const$ (no rotation) and the motion is one-dimensional. 

The pair of [[Equations of Motion]] in polar coordinates can be obtained by plugging in the polar coordinate equations into the two Newton's equations for $x$ and $y$, respectively. It is more wise, however, to take advantage of the conservation laws. From the point of view of the theory of differential equations, the two conservation laws are what is known as first [[Integral]]s. First integrals are the differential equations that are equivalent to the original ones but of the lower order. First integrals correspond to partially integrated original equations and thus contain free integration constants.

With the polar coordinates we have 
$$
\begin{align}
	v^2 = \dot{r}^2 + r^2 \dot{\theta}^2
\end{align}
$$
so in polar coordinates, conservation of energy reads:
$$
\begin{align}
	\frac{1}{2}m(\dot{r}^2+r^2\dot{\theta}^2) + U(r) = E
\end{align}
$$

The next good idea is to utilize the angular momentum equation to exclude $\dot{\theta}$. This brings us to the first order differential equation for find $r(t)$:

$$
\begin{align}
	\frac{1}{2}m\dot{r}^2 + \frac{l^2}{2mr^2}+U(r) = E
\end{align}
$$
Once $r(t)$ is found either analytically or numerically, one then employs the angular momentum equation to obtain $\theta(t)$ by analytic of numeric integration: 
$$
\begin{align}
	\theta(t) = \theta_0+\frac{l}{m}\int^t_0 \frac{dt'}{r^2(t')}
\end{align}
$$
The first order [[Ordinary Differential Equation]]  for finding $r(t)$ plays the key part in the theory of motion in the central potential. Let us see what are the general properties of the motion implied by this equation. First we note that the term 
$$
\begin{align}
	\frac{l^2}{2mr^2}
\end{align}
$$
is qualitatively similar to $U(r)$: it is a function of $r$ and thus can be formally interpreted as a certain repulsive central potential. That is why the term is called centrifugal potential. Correspondingly the minus gradient of the centrifugal potential is called centrifugal force . It makes then a perfect sense to combine the centrifugal potential with the genuine potential $U(r)$ into the effective potential
$$\begin{align} U_{eff}(r) = U(r)+\frac{l^2}{2mr^2} \end{align}$$
and write the $r(t)$ equation as
$$\begin{align} \frac{m\dot{r}^2}{2}+U_{eff}(r) = E \end{align}$$
If we differentiate this equation with repect to time we get
$$\begin{align} m\ddot{r}=F_{eff}(r), \; \; \; \; F_{eff}(r)=-\frac{d}{dr}U_{eff}(r)\end{align}$$
which has a simple and elegant physical interpretation. The radius $r$ evolves in time as if it is a coordinate of a one-dimensional particle of the mass $m$ moving in an external potential $U_{eff}$.