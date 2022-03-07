## Permanent Measurement
For a small enough time interval $\Delta t$ we have: $(\hbar = 1)$ 

$$\begin{gather}\hat \rho(t+\Delta t) = \hat \rho - i\Delta t[H,\hat \rho(t)]+ \mathcal{O}[(\Delta t)^2] \end{gather}$$

The probability to witness the same eigenvalue $\lambda$ after evolution is: 

$$\begin{gather} p_\lambda(\Delta t)=1-\mathcal{O}[(\Delta t)^2] \end{gather}$$
## Quantum Zeno Effect
Now let us fix some finite time interval $\tau$ and perform $N \gg 1$  measurements of the same quantity $A$, with the time interval $\Delta \tau = \tau/N$ between successive measurements. We see that in the limit $N\to\infty$  each successive measurement will deterministically yield one and the same eigenvalue $\lambda$ found in the very first measurement. This fact is known as quantum Zeno effect. 

The limit $N \to \infty$ corresponds to permanent observation. IF the eigenvalue $\lambda$ (that is measured in the first measurement) is non-degenerate then the system will not evolve. 

If the eigenvalue $\lambda$ is degenerate then the system keeps evolving. The law of this permanent measurement evolution is: 

$$\begin{gather} i\hbar \frac{\partial}{\partial t}\hat \rho = [H^{(\lambda)},\hat \rho] \\ H^{(\lambda)} = \hat P_\lambda H \hat P_\lambda \end{gather}$$
The second line is the projected onto the $\lambda$ subspace Hamiltonian. In the case of non-degenerate $\lambda$ $H^{(\lambda)}$ is just a number making $[H^{(\lambda)}, \hat \rho] \equiv 0$ and thus the suppression of any evolution. 

## Negative Measurement
