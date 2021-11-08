The general solution of the Equations of motion([[Classical Mechanics/Lagrangian Mechanics/Small Oscillations/Equations of Motion]]) reads: 

$$\begin{align} \vec x(t) = \sum_s \vec u_s \eta_s(t) \end{align}$$

where $$\begin{align} \eta_s(t) = C_s \text{Re} \ e^{i(\omega_st - \delta_s)} = C_s \cos(\omega_s t - \delta_s) \end{align}$$

Introduce new generalized coordinates, $\{\eta_s\}$ related to the original ones by: 
$$\begin{align} \vec x = \sum_s \vec u_s \eta_s \end{align}$$

Where the magnitudes of the [[Eigenvectors]] $\vec u_s$ are fixef by the normalization condition. Each term in this summation then represents the normal mode associated with each corresponding harmonic oscillator. 

$\vec u_s$ are obtained by solving the determinant problem given in [[Classical Mechanics/Lagrangian Mechanics/Small Oscillations/Equations of Motion]]. The frequencies emerge as the [[Eigenvalues]] of the mathematical problem. 

When all linear independent $\vec u_s$ are found we plug our new generalized coordinates into our [[Bilinearized Lagrangian]] to get: 

$$\begin{align}\mathcal L = \frac{1}{2} \sum_{s,s'} \left[\dot \eta_s \dot \eta_{s'} \vec u_s \cdot (\mathcal M \vec u_{s'} - \eta_s \eta_s' \vec u_s \cdot (\mathcal K\vec u_{s'}))\right] \end{align}$$

The eigenvectors have two crucial properties:
$$\begin{align} \vec u_s \cdot (\mathcal M \vec u_{s'}) = 0  \;\; \text{at} \;\; s \neq s' \\ \vec u_s \cdot (\mathcal K \vec u_{s'}) = 0  \;\; \text{at} \;\; s \neq s' \end{align}$$

Now we have: 
$$\begin{align}\mathcal L = \sum_s \frac{m_s}{2} \left[\dot \eta^2_s - \omega_s^2 \eta_s^2\right] \end{align}$$ with $$\begin{align} m_s = \vec u_s \cdot(\mathcal M \vec u_s)\\  \vec u_s \cdot(\mathcal K \vec u_s) = \omega^2_s \vec u_s \cdot(\mathcal M \vec u_s)\end{align}$$

Normalize the vectors $\vec u_s$ in such a way that:

$$\begin{align} \vec u_s \cdot(\mathcal M \vec u_s) = 1 \end{align}$$

So our Lagrangian takes the simple form: 

$$\begin{align}\mathcal L = \sum_s \frac{1}{2} \left[\dot \eta^2_s - \omega_s^2 \eta_s^2\right] \end{align}$$

The expression for the systems energy is
$$\begin{align} E = \sum_s \frac{1}{2} \left[\dot \eta^2_s + \omega_s^2 \eta_s^2\right] \end{align}$$
