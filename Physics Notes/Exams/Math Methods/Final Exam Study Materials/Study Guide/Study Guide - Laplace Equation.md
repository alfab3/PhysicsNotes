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

