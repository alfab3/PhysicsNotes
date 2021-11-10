Normal modes can be excited by applying a small external perturbation. We will confine ourselves with the case when such a perturbation corresponds to a time dependent generalized external potential term: 
$$\begin{align} L \rightarrow L - U_{ext}(t,\{q\}) \end{align}$$

Since the normal oscillations imply the limit of small amplitudes, the potential $U_{ext}$ should be Taylor expanded up to the first non-trivial terms about the position of equilibrium $\{q^{(0)}\}$: 
$$\begin{align} U_{ext}(t,\{q\}) \rightarrow U_{ext}(t,\{q^{(0)}\}) - \vec f(t) \cdot \vec x\end{align}$$

where: 
$$\begin{align} f_\alpha(t) = -\frac{\partial U_{ext}(t,\{q\})}{\partial q_\alpha}  \;\;\;\; (\text{at} \{q\}= \{q^{(0)}\}\end{align}$$

can be interpreted as the generalized force acting on the variable $x_\alpha$. The first term in the r.h.s is trivial - just a function of time. We omit it from now on.

We obtain the Lagrangian for the [[Normal Modes]] 
$$\begin{align} \mathcal L = \sum_s\left[\dot \eta _ 2^2/2 - \omega_s^2 \eta^2_s/2 + f_s(t) \eta_s\right] \end{align}$$

where $$\begin{align} f_s(t) = \vec f(t) \cdot \vec u_s \end{align}$$

Which has the meaning of the force acting on the normal variable $\eta_s$. The structure of the [[Lagrangian]] means that each normal mode moves independently from the others being driven by its own force. The equation of motion for the $s$-th normal mode is readily obtained. Below we omit the subscript $s$ for the mode(and also introduce the subscript $0$ to distinguish the [[Eigenfrequency]] of the mode from the frequency of the periodic driving force)
$$\begin{align}\ddot\eta +\omega_0^2 \eta = f(t)\end{align}$$

Whose solution takes the form: 
$$\begin{align} \eta = \eta_1 + \eta_2\end{align}$$

Where $\eta_1$ is the general solution to the [[Homogeneous Differential Equation]]
$$\begin{align} \ddot\eta_1 + \omega_0^2\ \eta_1 = 0 \end{align}$$ while $\eta_2$ is a particular solution to the original equation.

The solution can take 3 different forms:

$$\begin{align} \eta_1(t) = A\cos(\omega_0t-\phi) \equiv A\sin(\omega_0t - \tilde\phi) \equiv A_1\cos\omega_0t + A_2\sin\omega_0 t\end{align}$$

Let us find the solution $\eta_2$ for the most important case of a sinusoidal force
$$\begin{align} f(t) = a \cos \omega t \equiv \text{Re}\ ae^{i\omega t}\end{align}$$ 
It is convenient to look for the solution in the exponential form $$\begin{align} \eta_2 = \text{Re}\ Be^{i\omega t} \end{align}$$

This substitution translates the original differential equation into an algebraic equation for $B$ yielding 
$$\begin{align} B = \frac{a}{\omega_0^2 - \omega^2}\end{align}$$
and thus
$$\begin{align} \eta_2 = \frac{a}{\omega_0^2 - \omega^2} \cos\omega t\end{align}$$