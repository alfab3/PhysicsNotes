# Problem Solving Methods
### Boundary Conditions

#### Vacuum 
(point) - charges may exist and generate $\vec E$ field. That is, volumetric charge density (charge/volume) $\rho$ may be nonzero: 

$$\begin{gather} \nabla^2 \phi =\frac{1}{\epsilon_0}\rho \end{gather}$$

#### Conductor 
Net charge may not exist inside a conductor, and there is no $\vec E$-field. Any charges may exist only at the boundaries of a conducting body:

$$\begin{gather} \nabla \phi = 0 \\ \rho = 0 \\ \vec E = 0\end{gather}$$ $\sigma$ may be nonzero for the surface of the conductor
#### Electric Field
Apply Boundary conditions. The Laplace/Poisson Equation is an elliptical PDE ([[2nd Order Linear PDEs]]), therefore must apply [[Cauchy Boundary Conditions]], which state that(in free space with $\epsilon_0$ where the boundary is a sheet with surface charge $\sigma$, electric field above the surface is $E_a$ and below the surface is $E_b$): $$\begin{gather}E^\perp_a - E^\perp_b = \frac{\sigma}{\epsilon_0} \\ E^\parallel_a = E^\parallel_b\\ \text{which gives:} \\ [[\vec E]] = E_a - E_b = \frac{\sigma}{\epsilon_0}\hat n  \end{gather}$$ 

#### Electric Potential
For the potential, we have: $$\begin{gather} \phi_a - \phi_b = -\int^b_a \vec E \cdot dl \Rightarrow \phi_a = \phi_b \end{gather}$$ 

Since $$\begin{gather} -\int^b_a \vec E \cdot dl = 0 \end{gather}$$ because the tangential components of the electric field are equal. Now applying: $\vec E = -\nabla \phi$: $$\begin{gather} \nabla \phi_a - \nabla\phi_b = -\frac{\sigma}{\epsilon_0} \hat n \\ \Rightarrow \frac{\partial \phi_a}{\partial n} - \frac{\partial \phi_b}{\partial n} = -\frac{\sigma}{\epsilon_0}\end{gather}$$ 

#### Displacement field
For the $D$ field the boundaries: $$\begin{gather} D^\perp_a - D_b^\perp = \sigma_f \end{gather}$$ Where: $D_a = \epsilon_aE_a$ and $D_b = \epsilon_bE_b$

### Potential
#### Potential of a System of Point charges
This method will allow you to determine the potential from the point charges. Determine the Potential in the form(assuming there exists a system of  charges $q_i$ with some dielectric $\epsilon$): $$\begin{gather} \phi(\vec x) =\frac{1}{4\pi\epsilon} \sum_i \frac{q_i}{|r-r_i|}\end{gather}$$ Where: $q_i$ is the charge of the point charge, $r_i$ is the position of the point charge, $r$ is the test point, and $\epsilon$ is the dielectric constant of the medium the test point is in.

#### Solution to the Laplace Equation (Spherical Harmonics)

$$\begin{gather} Y^m_l(\theta,\varphi) = P_l(\cos\theta)e^{im\varphi} \end{gather}$$ 

Where $P_l(\cos\theta)$ are the [[Legendre Polynomials]]

In an axially symmetric problem $m=0$: 

$$\begin{gather}\phi(r,\theta,\varphi) = \sum^\infty_{l=0} [A_lr^l+B_lr^{-(l+1)}]P_l(\cos\theta) \end{gather}$$