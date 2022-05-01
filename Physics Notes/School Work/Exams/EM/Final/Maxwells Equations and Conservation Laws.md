## E and B fields from Potentials
>$$\begin{gather} \vec E = - \nabla \varphi - \frac{\partial \vec A}{\partial t} \\ \vec B = \nabla \times \vec A\end{gather}$$

# Gauge Transformations 
## Maxwell's Equations
$$\begin{gather} \nabla^2\Phi + \frac{\partial}{\partial t}(\nabla\cdot \vec A) = - \rho/\epsilon_0\\ \nabla^2\vec A - \frac{1}{c^2}\frac{\partial^2 \vec A}{\partial t^2} - \nabla\left(\nabla \cdot \vec A + \frac{1}{c^2}\frac{\partial \Phi}{\partial t}\right) = \mu_0 \vec J\end{gather}$$
Defined by: 

### Vector Potential
$$\begin{gather} \vec A \to \vec A' = \vec A + \nabla\Lambda \end{gather}$$
Where $\Lambda$ is some scalar function

### Scalar Potential
$$\begin{gather} \Phi \to \Phi' = \Phi - \frac{\partial \Lambda}{\partial t}\end{gather}$$
## Lorenz Gauge
$$\begin{gather} \nabla \cdot \vec A' + \frac{1}{c^2}\frac{\partial \Phi'}{\partial t} = 0 = \nabla \cdot \vec A + \frac{1}{c^2}\frac{\partial \Phi}{\partial t} + \nabla^2\Lambda - \frac{1}{c^2}\frac{\partial^2 \Lambda}{\partial t^2}  \end{gather}$$

## Coulomb Gauge
$$\begin{gather} \nabla \cdot \vec A = 0 \end{gather}$$

#### Poisson Equation 
$$\begin{gather} \nabla^2 \Phi = -\rho/\epsilon_0 \\ \Phi(\vec x,t) = \frac{1}{4\pi\epsilon_0} \int\frac{\rho(\vec x',t)}{|\vec x - \vec x'|} d^3x'\end{gather}$$
#### Vector Potential 
$$\begin{gather} \nabla^2 \vec A - \frac{1}{c^2} \frac{\partial^2 \vec A}{\partial t^2} = -\mu_0\vec J + \frac{1}{c^2} \nabla\frac{\partial \Phi}{\partial t}\end{gather}$$
##### Current Density
$$\begin{gather} \vec J = \vec J_l + \vec J_t \end{gather}$$
$\vec J_l$ is longitudinal current $\nabla \times \vec J_l = 0$ 
$\vec J_t$ is transverse current $\nabla \cdot \vec J_t = 0$

Gives us: 
$$\begin{gather} J_l (\vec x,t) = -\frac{1}{4\pi} \nabla\int \frac{\nabla'\cdot \vec J(\vec x,t)}{|\vec x - \vec x'|}\end{gather}$$
$$\begin{gather} J_t (\vec x,t) = -\frac{1}{4\pi} \nabla \times \nabla \times \int \frac{\vec J(\vec x,t)}{|\vec x - \vec x'|}\end{gather}$$
Which with $$ \begin{gather}\frac{1}{c^2} \nabla \frac{\partial \Phi}{\partial t} = \mu_0 J_l \end{gather}$$
Allows us to write the source for the equation for $\vec A$ 
$$\begin{gather} \nabla^2 \vec A - \frac{1}{c^2}\frac{\partial^2 \vec A}{\partial t^2} = \mu_0 \vec J_t \end{gather}$$
#### Fields 
$$\begin{gather} \vec E = - \frac{\partial A}{\partial t} \\ \vec B =\nabla \times \vec A \end{gather}$$
