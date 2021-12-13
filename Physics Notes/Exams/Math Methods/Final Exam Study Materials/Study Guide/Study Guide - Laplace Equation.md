# Definition
The Laplace equation for a scalar field $\Phi(\vec x)$: 

$$\begin{gather} \nabla^2\Phi = 0 \end{gather}$$

Where $\nabla^2$ is the Laplacian

# Solution
The solution takes the form: 

$$\begin{gather} \Phi(r,\theta,\varphi) = \sum_{l,m}[\alpha_{lm}r^l + \beta_{lm}r^{-(l+1)}] Y_{lm}(\theta, \varphi) \end{gather}$$

Where $Y_{lm}$ are the Spherical Harmonics and $\{\alpha_l, \beta_l\}^\infty_{l=1}$ are found from boundary conditions.

The spherical harmonics are given by:

$$\begin{gather} Y^m_l(\theta,\varphi) = P_l(\cos\theta)e^{im\varphi} \end{gather}$$ 

Where $P_l(\cos\theta)$ are the [[Legendre Polynomials]]

In an axially symmetric problem $m=0$: 

$$\begin{gather}\phi(r,\theta,\varphi) = \sum^\infty_{l=0} [A_lr^l+B_lr^{-(l+1)}]P_l(\cos\theta) \end{gather}$$

## Solving for $\phi$
1) Apply Boundary conditions. The Laplace/Poisson Equation is an elliptical PDE ([[2nd Order Linear PDEs]]), therefore must apply [[Cauchy Boundary Conditions]], which state that(in free space with $\epsilon_0$ where the boundary is a sheet with surface charge $\sigma$, electric field above the surface is $E_a$ and below the surface is $E_b$): $$\begin{gather}E^\perp_a - E^\perp_b = \frac{\sigma}{\epsilon_0} \\ E^\parallel_a = E^\parallel_b\\ \text{which gives:} \\ E_a - E_b = \frac{\sigma}{\epsilon_0}\hat n  \end{gather}$$ For the potential, we have: $$\begin{gather} \phi_a - \phi_b = -\int^b_a \vec E \cdot dl \Rightarrow \phi_a = \phi_b \end{gather}$$ Since $$\begin{gather} -\int^b_a \vec E \cdot dl = 0 \end{gather}$$ because the tangential components of the electric field are equal. Now applying: $\vec E = -\nabla \phi$: $$\begin{gather} \nabla \phi_a - \nabla\phi_b = -\frac{\sigma}{\epsilon_0} \hat n \\ \Rightarrow \frac{\partial \phi_a}{\partial n} - \frac{\partial \phi_b}{\partial n} = -\frac{\sigma}{\epsilon_0}\end{gather}$$ For the $D$ field the boundaries: $$\begin{gather} D^\perp_a - D_b^\perp = \sigma_f \end{gather}$$ Where: $D_a = \epsilon_aE_a$ and the same for $b$
2) Note: You won't always need this step, this step is only for cases with charges. If there are no charges skip ahead to part 3. This method will allow you to determine the potential from the point charges. Determine the Potential in the form(assuming there exists a system of  charges $q_i$ with some dielectric $\epsilon$): $$\begin{gather} \phi(\vec x) =\frac{1}{4\pi\epsilon} \frac{q_i}{|r-r_i|}\end{gather}$$ Where: $q_i$ is the charge of the point charge, $r$ is the position of the point charge, $r_i$ is the test point, and $\epsilon$ is the dielectric constant of the area where $r_i$ is. 
3) 