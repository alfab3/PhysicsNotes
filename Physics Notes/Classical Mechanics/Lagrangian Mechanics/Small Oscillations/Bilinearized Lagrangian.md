Systems of particles interacting through central potentials:
$$\begin{align} \mathcal{L} = T - U \\ T = \sum^N_{i=1} \frac{m_i\dot {\mathbf r_i}}{2} \\ U = \sum_{i < j}U_{ij}(|\mathbf r_i - \mathbf r_j|)\end{align}$$

Any type of potential energy depending on positions of particles is equally good. The crucial circumstance is that our Lagrangian does not have terms linearly proportional to velocities.

First we make certain observations concerning the form of the Lagrangian in new generalized coordinates, $\{q_{\alpha}\}$ related to the [[Cartesian Coordinates]] by some functions: 

$$\begin{align} q_\alpha = f_\alpha(\{\mathbf r_i\}) \\ \dot q_{\alpha} = \sum^N_{i=1} \frac{\partial f_\alpha}{\partial \mathbf r} \cdot \mathbf {\dot{r}}_i \end{align}$$

Hence $\mathbf{\dot{r}}$ is a linear function of $\dot q$'s with some coefficients that are functions of $q$'s. Correspondingly the form of the Lagrangian in new coordinates is: 

$$\begin{align} \mathcal L = \frac{1}{2} \sum_{\alpha\beta}m_{\alpha\beta}\dot q_\alpha \dot q_\beta - U(\{q\})\end{align}$$

where $m_{\alpha\beta}$ is a [[Symmetric Matrix]] that depends on $q$'s , but not on $\dot q$'s

By definition, the equilibrium is the time independent solution of the [[Classical Mechanics/Lagrangian Mechanics/Small Oscillations/Equations of Motion]]: 

$$\begin{align} q_\alpha (t) \equiv q_\alpha^{(0)}, \;\; \dot q_\alpha(t) \equiv 0 \end{align}$$

In accordance with the Lagrange equations, the equilibrium value $q_\alpha^{(0)}$ are found from the system of equations (for all $\alpha$'s')
$$\begin{align} \frac{\partial U(\{q^{(0)}\})}{\partial q_\alpha^{(0)}} = 0 \end{align}$$
Introducing the deviations of the coordinates from their equilibrium positions $$\begin{align} x_\alpha (t) = q_\alpha(t) - q_\alpha^{(0)}, \;\;\;\;\;\;\;\;\; \dot x_\alpha = \dot q_\alpha \end{align}$$ and taking into account that we are interested only in the limit of small x's, we expand the [[Lagrangian]] as the [[Taylor Series]] in powers of $x$'s up to the leading terms. In the kinetic-energy term, this amounts to requiring that $$\begin{align} m_{\alpha\beta}(\{q\}) = m_{\alpha\beta}(\{q^{(0)}\})\end{align}$$ 

In the potential energy term, we have to expand up to the second-order partial derivatives, since the first-order derivatives are equal to zero by the condition of the equilibrium, and the first term of the Taylor series is simply a constant that should be immediately omitted because of its irrelevance for the dynamics. We arrive at the bilinearized Lagrangian:

$$\begin{align} \mathcal L = (1/2) \sum_{\alpha, \beta}[m_{\alpha\beta}\dot x_\alpha \dot x_\beta - k_{\alpha, \beta} x_\alpha x_\beta] \end{align}$$

In which $m_{\alpha\beta}$ and $k_{\alpha\beta}$ are certain constant matrices, and, in particular 
$$\begin{align} k_{\alpha\beta} = \frac{\partial^2 U(\{q^{(0)}\})}{\partial q_\alpha^{(0)}\partial q_\beta^{(0)}}\end{align}$$

The matrix $m_{\alpha\beta}$ is symmetric by construction. We will assume both $m_{\alpha\beta}\; \text{and} \; k_{\alpha\beta}$ are symmetric.

In vector matrix notation:

$$\begin{align} \vec x = (x_1,x_2,x_3,...) \\ (\mathcal M)_{\alpha\beta} = m_{\alpha\beta}, \;\;\;\;\;\;\;\; (\mathcal K)_{\alpha\beta} = k_{\alpha\beta} \\ \mathcal L = \frac{1}{2} [\dot{\vec{x}} \cdot(\mathcal M\dot{\vec{x}})-\vec x \cdot (\mathcal K\vec x)] \end{align}$$