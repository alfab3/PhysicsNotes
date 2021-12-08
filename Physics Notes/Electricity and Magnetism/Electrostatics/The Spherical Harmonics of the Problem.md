Let us know the [[Eigenvalues]] problem:

$$\begin{gather} \hat{\mathcal L}^2 Y_{lm}(\theta,\phi) \equiv \frac{-1}{\sin\theta} \frac{\partial}{\partial \theta} \sin\theta\frac{\partial Y_{lm}}{\partial \theta}-\frac{1}{\sin^2\theta}\frac{\partial^2 Y_{lm}}{\partial \phi^1} = \lambda_{lm}Y_{lm}(\theta,\phi)  \end{gather}$$

where $Y_{lm}$ represents the [[Spherical Harmonics]]. This leads to the structure of the Legendre Polynomials, which then gives us the solution to the [[Laplace's Equation]] expressed using spherical harmonics: 

$$\begin{gather} \Phi (r, \theta, \phi) = \sum_{l=0}^\infty \sum^l_{m=-l}[A_{l,m}r^l+B_{lm} r^{-(l+1)}]Y^m_{l}(\theta,\phi)\end{gather}$$

where $\{A_{l,m},B_{l,m}\}$ are coefficients that must be determined by boundary conditions, and $$\begin{gather} Y^m_l(\theta,\phi) = P_l(\cos\theta) e^{im\phi}\end{gather}$$

We can rely on a lot of problems to have axial symmetry:

$$\begin{gather}\Phi(r,\theta,\phi) = \sum^{\infty}_{l=0}[A_lr^l+B_lr^{-(l+1)}]P_l(\cos\theta) \end{gather}$$