With [[Vectors]] notation, the Lagrange equation of motion reads
$$\begin{align} \frac{d}{dt} \frac{\partial \mathcal L}{\partial \dot{\vec{x}}} = \frac{\partial \mathcal L}{\partial \vec x} \end{align}$$

Plugging in our [[Bilinearized Lagrangian]] we find that: 

$$\begin{align}\frac{\partial \mathcal L}{\partial \dot{\vec{x}}} = \mathcal M \dot{\vec x},\;\;\;\;\;\;\; \frac{\partial \mathcal L}{\partial \vec x} = - \mathcal Kx \end{align}$$

and get the equation of motion in the form
$$\begin{align} \mathcal M \ddot {\vec x} + \mathcal K \vec x = 0\end{align}$$

Mathematically, we are dealing with a [[Second Order Linear ODEs]] with [[Constant Coefficients]], the general solution to which comes in the form of a [[Linear Combination]] of special solutions: 
$$\begin{align} \vec x = \sum_s C_s\vec a_s(t)\end{align}$$

Here $C_s$ are arbitrary coefficients and $$\begin{align} \vec a_s(t) = \vec u_s \text{Re}\ e^{i(\omega_s)t - \delta_s} = \vec u_s cos(\omega_s t - \delta _s) \end{align}$$

In the special solution, where $\vec u_s$ is a real [[Eigenvectors]], $\omega_s$ is an [[Eigenfrequency]], and $\delta_s$ is an arbitrary phase shift. In view of the special form of time-dependent factor the linear differential equation for $\vec a_s(t)$, 
$$\begin{align} \mathcal M \ddot{\vec{a}}_s+ \mathcal K \vec a_s = 0 \end{align}$$
reduces to linear algebraic equation for $\vec u_s$:
$$\begin{align} (\mathcal K - \omega^2_s \mathcal M) \vec u_s = 0 \end{align}$$

which has non-trivial solutions for special values of the parameter $\omega_s$ , when the determinant of the matrix is equal to zero  $$\begin{align} \text{det}(\mathcal K - \omega_s^2 \mathcal M) = 0 \end{align}$$

The latter requirement forms the equation for finding [[Eigenfrequency]] $\omega_s$, the so called characteristic equation. For each [[Eigenfrequency]] $\omega_s$ then gives one or more linear independent eigenvectors. The total number of linear independent eigenvectors is always equal to the dimensionality of the original vector $\vec x$.