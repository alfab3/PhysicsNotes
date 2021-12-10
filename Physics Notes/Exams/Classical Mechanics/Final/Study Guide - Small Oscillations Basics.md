# Bilinearized Lagrangian

[[Bilinearized Lagrangian]]

A [[Lagrangian]] that deals with microscopic systems of particles.

$$\begin{gather} \mathcal L = T-U, & T = \sum^N_{i=1} \frac{m_i\dot r_i^2}{2}, & U = \sum_{i < j}U_{ij}(|\vec r_i - \vec r_j|)\end{gather}$$


Writing in Matrix Form: 

$$\begin{align} \mathcal L = \frac{1}{2} [\dot{\vec{x}} \cdot(\mathcal M\dot{\vec{x}})-\vec x \cdot (\mathcal K\vec x)] \end{align}$$

## Equations of Motion

With [[Vectors]] notation, the Lagrange equation of motion ([[Euler-Lagrange Equation]]) reads
$$\begin{align} \frac{d}{dt} \frac{\partial \mathcal L}{\partial \dot{\vec{x}}} = \frac{\partial \mathcal L}{\partial \vec x} \end{align}$$

Plugging in our [[Bilinearized Lagrangian]] we find that: 

$$\begin{align}\frac{\partial \mathcal L}{\partial \dot{\vec{x}}} = \mathcal M \dot{\vec x},\;\;\;\;\;\;\; \frac{\partial \mathcal L}{\partial \vec x} = - \mathcal Kx \end{align}$$

and get the equation of motion in the form
$$\begin{align} \mathcal M \ddot {\vec x} + \mathcal K \vec x = 0\end{align}$$

This is a [[Second Order Linear ODEs]] with [[Constant Coefficients]], the general solution to which comes in the form of a linear combination:

$$\begin{align} \vec x = \sum_s C_s\vec a_s(t)\end{align}$$

Here $C_s$ are arbitrary coefficients and $\vec a_s(t)$ is defined as:
$$\begin{align} \vec a_s(t) = \vec u_s \text{Re}\ e^{i(\omega_s)t - \delta_s} = \vec u_s cos(\omega_s t - \delta _s) \end{align}$$

In the special solution, where $\vec u_s$ is a real [[Eigenvectors]], $\omega_s$ is an [[Eigenfrequency]], and $\delta_s$ is an arbitrary [[Phase]] shift. In view of the special form of time-dependent factor the linear differential equation for $\vec a_s(t)$, 
$$\begin{align} \mathcal M \ddot{\vec{a}}_s+ \mathcal K \vec a_s = 0 \end{align}$$
reduces to linear algebraic equation for $\vec u_s$:
$$\begin{align} (\mathcal K - \omega^2_s \mathcal M) \vec u_s = 0 \end{align}$$

which has non-trivial solutions for special values of the parameter $\omega_s$ , when the determinant of the matrix is equal to zero  $$\begin{align} \text{det}(\mathcal K - \omega_s^2 \mathcal M) = 0 \end{align}$$

The latter requirement forms the equation for finding [[Eigenfrequency]] $\omega_s$, the so called characteristic equation. For each [[Eigenfrequency]] $\omega_s$ then gives one or more linear independent eigenvectors. The total number of linear independent eigenvectors is always equal to the dimensionality of the original vector $\vec x$.

# Normal Modes

## Form of the Solution

The general solution of the Equations of motion([[Classical Mechanics/Lagrangian Mechanics/Small Oscillations/Equations of Motion]]) reads: 

$$\begin{align} \vec x(t) = \sum_s \vec u_s \eta_s(t) \end{align}$$

where $$\begin{align} \eta_s(t) = C_s \text{Re} \ e^{i(\omega_st - \delta_s)} = C_s \cos(\omega_s t - \delta_s) \end{align}$$

Introduce new generalized coordinates, $\{\eta_s\}$ related to the original ones by: 
$$\begin{align} \vec x = \sum_s \vec u_s \eta_s \end{align}$$


Where the magnitudes of the [[Eigenvectors]] $\vec u_s$ are fixed by the normalization condition. Each of these terms are independent of each other. Each term in this summation then represents the normal mode associated with each corresponding harmonic oscillator. 

## Eigenvectors

$\vec u_s$ are obtained by solving the determinant problem given in [[Classical Mechanics/Lagrangian Mechanics/Small Oscillations/Equations of Motion]]. The frequencies emerge as the [[Eigenvalues]] of the mathematical problem. 


The eigenvectors have two crucial properties:
$$\begin{align} \vec u_s \cdot (\mathcal M \vec u_{s'}) = 0  \;\; \text{at} \;\; s \neq s' \\ \vec u_s \cdot (\mathcal K \vec u_{s'}) = 0  \;\; \text{at} \;\; s \neq s' \end{align}$$

Now we have: 
$$\begin{align}\mathcal L = \sum_s \frac{m_s}{2} \left[\dot \eta^2_s - \omega_s^2 \eta_s^2\right] \end{align}$$ with 

$$\begin{gather} m_s = \vec u_s \cdot(\mathcal M \vec u_s) \end{gather}$$

From the [[Eigenvectors]] equation:
$$ \begin{gather}\vec u_s \cdot(\mathcal K \vec u_s) = \omega^2_s \vec u_s \cdot(\mathcal M \vec u_s)\end{gather}$$

Normalize the vectors $\vec u_s$ in such a way that:

$$\begin{align} \vec u_s \cdot(\mathcal M \vec u_s) = 1 \end{align}$$

## Lagrangian and Energy (with $\eta$)

So our Lagrangian takes the simple form: 

$$\begin{align}\mathcal L = \sum_s \frac{1}{2} \left[\dot \eta^2_s - \omega_s^2 \eta_s^2\right] \end{align}$$

The expression for the systems energy is
$$\begin{align} E = \sum_s \frac{1}{2} \left[\dot \eta^2_s + \omega_s^2 \eta_s^2\right] \end{align}$$

Which gives us the condition: 

$$\begin{gather} \omega_s^2 > 0 \end{gather}$$

which is the necessary and sufficient condition to have a local energy minimum at the point of equilibrium. 

Relevant Homework Problems:

[[Problem 28]]

[[Problem 29]]




