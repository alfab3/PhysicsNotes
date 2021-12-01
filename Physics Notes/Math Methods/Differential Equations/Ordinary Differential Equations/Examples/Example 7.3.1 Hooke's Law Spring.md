A mass $M$ attached to a Hooke's Law spring is an oscillatory motion. Letting y ve the displacement of the mass from its equilibrium position, Newton's law of motion takes the form
$$
M\frac{d^2y}{dt^2}=-ky
$$
which is an [[Ordinary Differential Equation]] of the form $y''+a_0y=0$, with $a_0=+k/M$. The general solution to this ODE is of the form 
$$
C_1e^{m_1t}+C_2e^{m_2t}
$$
where $m_1$ and $m_2$ are the solutions of the algebraic equation $m^2+a_0=0$.

The values of $m_1$ and $m_2$ are $i\omega$, where $\omega = \sqrt{k/M}$, so the ODE has solution 
$$
y(t)=C_1e^{+i\omega t}+C_2e^{-i\omega t}
$$
Since the ODE is homogeneous, we may alternatively describe its general solution using arbitrary linear combinations of the above two terms. This permits us to combine them to obtain forms that are real and therefore appropriate to the current problem. Noting that 
$$
\frac{e^{iwt}+e^{-iwt}}{2}=\cos\omega t \; and \; \frac{e^{iwt}-e^{-iwt}}{2}=\sin\omega t
$$
a convenient alternate form is
$$
y(t)=C_1 \cos \omega t + C_2 \sin \omega t
$$
The solution to a specific [[Oscillation]] problem will now involve fitting the coefficients $C_1$ and $C_2$ to the initial conditions, as for example $y(0)$ and $y'(0)$