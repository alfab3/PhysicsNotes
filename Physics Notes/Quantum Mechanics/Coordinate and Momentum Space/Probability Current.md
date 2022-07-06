The [[Continuity Equation]] is defined as:

$$\begin{gather} \partial_t \rho(\vec r,t) = - \nabla\cdot\vec j(\vec r, t) \end{gather}$$

To see that this infers that [[Charge Conservation]] is local, one applies the [[Divergence Theorem]]. For any volume $V$:

$$\begin{gather} \partial_t\int_V d^3 r \rho(\vec r,t) = - \int_V d^3r\ \nabla \cdot \vec j(\vec r,t) \\ \frac{d}{dt} Q = -\oint d\vec A\cdot \vec j(\vec r,t)\end{gather}$$

where Q is the charge within the volume $V$. By considering arbitrarily small volumes, this shows that the change in charge within that volume can be identified with the [[Current Density]] $\vec j$ exiting the surface of the volume. 

[[Schrodinger Equation]] allows one to identify both the charge and current densities. First, consider Schrodinger's wave equation and its [[Complex Conjugate]]

$$\begin{gather} \frac{-\hbar^2 \nabla_2^2}{2m}\psi^*(\vec r_1,t_1) \psi(\vec r_2,t_2) + V(\vec r_2,t_2)\psi^*(\vec r_1,t_2)\psi(\vec r_2,t_2) = -i\hbar\frac{\partial}{\partial t_2}\psi^*(\vec r_1,t_1)\psi(\vec r_2,t_2) \\ \frac{-\hbar^2 \nabla_1^2}{2m}\psi^*(\vec r_1,t_1) \psi(\vec r_2,t_2) + V(\vec r_1,t_1)\psi^*(\vec r_1,t_2)\psi(\vec r_2,t_2) = -i\hbar\frac{\partial}{\partial t_1}\psi^*(\vec r_1,t_1)\psi(\vec r_2,t_2) \end{gather}$$
The second equation is found by taking the complex conjugate of the first equation then switching 1 $\leftrightarrow$ 2. Subtracting the two equations and using the fact that $\nabla_1^2 - \nabla_2^2 = (\nabla_1-\nabla_2)(\nabla_1+\nabla_2)$, dividing by $i\hbar$ and setting $\vec r_1 = \vec r_2$ and $t_1 = t_2$.


$$\begin{gather} \vec j (\vec r,t)=-\frac{i\hbar}{2m}\psi^* (\vec r,t) \nabla\psi(\vec r,t) + \frac{i\hbar}{2m}[\nabla\psi^*(\vec r,t)] \psi(\vec r,t)\end{gather}$$

If one associates $i\hbar \nabla/m$ with the [[Velocity]], then the current looks like a velocity density.

