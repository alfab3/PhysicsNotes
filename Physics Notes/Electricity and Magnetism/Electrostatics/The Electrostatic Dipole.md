Let us consider two opposite point charges and assume we are interested in finding $\phi(\vec x)$ at some point since there is obviously an axial symmetry with respect to the axis that connects the two charges, it is useful to choose it as our z-axis, with the origin at the middle point between the two charges such that

$$\begin{gather} \phi(\vec x) = \phi(r,\theta,\phi_ = \sum^\infty_{l=0}[A_lr^l+B_lr^{-(l+1)}]P_l(\cos\theta)\end{gather}$$

which is the form of the [[Solution of Laplace Equation]]

![[electric dipole.png]]
we would like to compute the coefficients $A_l$ and $B_l$, Before doing the actual calculation, let us note that we mus distinguish between two limits:

$r \to 0$ or more generally $r \ll d$. Here since $\phi \to \text{const}$ we see that $\{B_l\}=0$

$r \to \infty$ (or more generally $r \gg d$): 
Gere since $\phi \to 0$ we see that $\{A_l\}=0$

This means the solution is not uniform. That is, the unavoidable singularities at $r = \pm d$ (due to the point charges) give rise to two separate expansions in terms of spherical harmonics ("near-field" and "far field")

In order to find $A_l$ and $B_l$, lets us recall basic electrostatics, where we obtain the [[Electric Potential]] through "superposition" of the potential induced by the two point charges:

$$\begin{gather} \phi(\vec x) \frac{q}{4\pi\epsilon_0}\left[\frac{1}{\sqrt{r^2+d^2-2rd\cos\theta}} - \frac{1}{\sqrt{r^2+d^2+2rd\cos\theta}}\right] \end{gather}$$

