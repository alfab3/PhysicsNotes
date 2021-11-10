Dissipative processes cannot be directly described by Lagrange Formalism. The dissipation(friction) can be readily taken into account in the equations of motion. For the harmonic oscillator this is done by adding a force linearly proportional (and oppositely directed) to the [[Velocity]]:

$$\begin{align}\ddot \eta + \omega_0^2 \eta + \gamma \dot\eta = f(t)\end{align}$$

The proportionality coefficient $\gamma$ is called the friction coefficient. It has the same dimensions as $\omega_0$. While the term with $\omega_0$ is responsible for the oscillations, the term with $\gamma$ leads to damping of the oscillatory motion. 

The solution can be written as $\eta = \eta_1 + \eta_2$ which is a super position of the general solution of the [[Homogeneous Differential Equation]] and a particular solution, $\eta_2$ of the original equation. 

The physics of the dissipative problem, however is such that the general solution of the homogeneous equation vanishes with time, so that after a certain transient regime only the particular solution survives. That is why finding the particular solution is of prime importance, and we begin our analysis with it. Assuming that the force is given by
$$\begin{align} f(t) = a\cos\omega t\equiv \text{Re}\ ae^{i\omega t} \end{align}$$
we look for the solution: 

$$\begin{align}B = \frac{a}{\omega_0^2 - \omega^2 + i \gamma\omega} \;\;\;\;\;\;\; \Rightarrow \;\;\;\;\;\;\;\;|B| = \frac{a}{\sqrt{(\omega_0^2-\omega^2)^2+\gamma^2\omega^2}} \end{align}$$

If $\gamma \ll \omega_0$ then the amplitude $|B|$ has a peaked shape with the characteristic width of the order of $\gamma$. The resonance takes place at the frequency $\omega_R \approx \omega_0$ and the amplitude at resonance is perfectly approximated by the value of $|B|$ at $\omega = \omega_0$:

$$\begin{align}|B|_R \approx \frac{a}{\omega_0 \gamma} \end{align}$$

With increasing $\gamma$, the peak broadens and its amplitude decreases. At $\gamma \approx \omega_0$ The position of the peak significantly shifts from $\omega_0$ to lower frequencies, as is seen from the exact formula for the resonance frequency (the frequency corresponding to the maximal $|B|$): 

$$\begin{align} \omega_R = \sqrt{\omega_0^2 - \gamma^2/2}\end{align}$$ From this relation we also see that the position of the peak reaches zero [[Frequency]] at $\gamma = \sqrt{2}\omega_0$