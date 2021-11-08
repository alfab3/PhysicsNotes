Systems of particles interacting through central potentials:
$$\begin{align} \mathcal{L} = T - U \\ T = \sum^N_{i=1} \frac{m_i\dot {\mathbf r_i}}{2} \\ U = \sum_{i < j}U_{ij}(|\mathbf r_i - \mathbf r_j|)\end{align}$$

Any type of potential energy depending on positions of particles is equally good. The crucial circumstance is that our Lagrangian does not have terms linearly proportional to velocities.

First we make certain observations concerning the form of the Lagrangian in new generalized coordinates, $\{q_{\alpha}\}$ related to the [[Cartesian Coordinates]] by some functions: 

$$\begin{align} \dot q_{\alpha} = \sum^N_{i=1} \frac{\partial f_\alpha}{\partial \mathbf r} \cdot \mathbf {\dot{r}}_i \end{align}$$

Hence $\mathbf{\dot{r}}$ is a linear function of $\dot q$'s with some coefficients that are functions of $q$'s. Correspondingly the form of the Lagrangian in new coordinates is: 

$$\begin{align} \mathcal L = \frac{1}{2} \sum_{\alpha\beta}m_{\alpha\beta}\dot q_\alpha \dot q_\beta - U(\{q\})\end{align}$$

where $m_{\alpha\beta}$ is a [[Symmetric Matrix]] that depends on $q$'s , but not on $\dot q$'s

By definition 