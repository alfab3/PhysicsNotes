## Schrodinger Equation
$$\begin{gather} -\frac{1}{2m} \psi''(x) + [V(x)-E]\psi(x) = 0 \\ V(x) = \frac{m\omega^2x^2}{2} \end{gather}$$
Where $\omega$ is the frequency of oscillations and $m$ is the mass


Define non-dimensional values: 
$$\begin{gather} \epsilon = (2/\omega) E \;\; \text{(Energy)} \\ \xi = \sqrt{m\omega}x \;\; \text{(Coordinate)} \\ \tilde{\psi} = \psi/(m\omega)^{1/4} \\ \int|\psi|^2 dx = 1 \Leftrightarrow \int|\tilde\psi|^2 d\xi =1 \end{gather}$$

$$\begin{gather} \psi''(\xi)+(\epsilon - \xi^2)\psi(\xi) = 0 \end{gather}$$



#### Wavefunction
$$\begin{gather} \psi_n(\xi) = C_nH_n(\xi)e^{-\xi^2/2} \\ \\ C_n = (\sqrt{\pi}\ 2^n n!)^{-1/2} \;\; (\xi - \text{representation})\\ \\ C_n = (\sqrt{\pi}\ 2^n n!)^{-1/2}(m\omega)^{1/4} \;\; (x - \text{representation})\end{gather}$$

$H_n(\xi)$ represents the Hermite Polynomials the first 4 are written as:

$$\begin{gather} H_0 = 1 \\ H_1 = 2\xi \\ H_2 = 4\xi^2 - 2 \\ H_3 = 8\xi^3 - 12\xi \\ H_4 = 16\xi^4 - 48\xi^2 + 12\end{gather}$$

## Energy 
$$\begin{gather} E_n = \hbar \omega(n+1/2) \;\; (n=0,1,2,\ldots) \end{gather}$$

## Time Dependent State
$$\begin{gather} \chi(x,t) = e^{-i\omega t/2} \sum_{n=0}^{\infty} \chi_n e^{-inwt}\psi_n(x) \;\; \chi_n = \int_{-\infty}^\infty 
 \psi_n \chi(x,0)\end{gather}$$