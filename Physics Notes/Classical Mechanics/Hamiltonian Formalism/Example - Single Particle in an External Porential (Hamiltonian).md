Let us derive the Hamiltonian ([[Hamiltonian Function and Hamilton's Equations]]) of a single particle in an external potential. Starting from the Lagrangian 
$$\begin{gather}\mathcal L = \frac{m\dot{\vec r}^2}{2} - U(\vec r) \end{gather}$$
we find the vector of the generalized momentum:

$$\begin{gather} \vec p = \frac{\partial L}{\partial \dot{\vec r}}=m\dot{\vec{r}}\end{gather}$$

The generalized momentum coincides with what we previously introduced as the [[Classical Mechanics/Motion/Linear Momentum]]. The Hamiltonian of the system is then $$\begin{gather} H = \frac{\vec{p}^2}{2m}+U(\vec r) \end{gather}$$
and the Hamiltonian's equations are 
$$\begin{gather} \dot {\vec{r}} = \vec p/m, \;\;\; \dot{\vec p} = -\frac{\partial U}{\partial r} = \vec F(\vec r) \end{gather}$$

The generalization for the system of $N$ particles interacting through pair potentials is as follows

$$\begin{gather}H = \sum^N_{j=1}\frac{\vec p^2_j}{2mj} + \sum_{i<j}U_{ij}(|\vec r_i - \vec r_j|) \\ \dot{\vec r} = \vec p_i/m_i, \;\;\; \dot{\vec{p}}_i = \sum_{j\neq i}\vec{F}_{ij},\;\;\; \vec{F}_{ij} = -\frac{\partial U_{ij}}{\partial \vec{r}_i}\end{gather}$$

For a less intuitive example, note that in the magnetic field the generalized momentum, $\vec P$, does not coincide with the linear momentum $\vec p$. It is easy to verify that in a uniform magnetic field $\vec B$ one has 
$$\begin{gather}\vec P = \vec p +\frac{e}{2}\vec B \times \vec r \\ H(\vec P, \vec r) = \frac{1}{2m}(\vec P -\frac{e}{2}\vec B\times \vec r)^2\end{gather}$$