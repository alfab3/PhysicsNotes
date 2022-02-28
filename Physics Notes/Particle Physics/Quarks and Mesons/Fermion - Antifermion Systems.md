## Fermions
Spin (1/2) $\ket{s, m_s} = \ket{1/2,\pm 1/2}$
Fermion wavefunctions are anti-symmetric
$m$ is the angular momentum projection onto the z-axis

#### Examples of Fermion - Antifermion systems
Positronium - $e^-e^+$
Muonium - $\mu^-\mu^+$
Quarkonium - $q \bar{q}$
A system of a particle and a antiparticle

## Spin
Orbital angular momentum $L$, total angular momentum $J$, spin $S$
Total angular momentum is defined as:

$$\begin{gather} J = L \oplus S = |L-S|,|L-S+1|,...|L+S| \end{gather}$$

Spin:
$$\begin{gather} S_1=1/2, \;\;\; S_2=1/2 \\ S = S_1 \oplus S_2 = \frac{1}{2} \oplus \frac{1}{2} = 0 \;\; \text{or} \;\; 1\end{gather}$$
This system can be aligned: 
$$\begin{gather} \uparrow_1 \uparrow_2, \; \uparrow_1 \downarrow_2,\; \downarrow_1 \uparrow_2, \; \downarrow_1 \downarrow_2\end{gather}$$
where: 
$S = 0, m_s = 0 \;\; 1$
$S = 1, m_s = +1,0,-1 \;\; 3$

Symmetric combination:  (spin 1)
$$\begin{gather} \frac{1}{\sqrt{2}} [\ket{\uparrow_1 \downarrow_2}+\ket{\downarrow_1 \uparrow_2}]\end{gather}$$
Anti-symmetric combination: (spin 0)
$$\begin{gather} \frac{1}{\sqrt{2}}[\ket{\uparrow_1\downarrow_2} - \ket{\downarrow_1 \uparrow_2}] \end{gather}$$
### Clebsch Gordan Coefficients 
$$\begin{gather} \ket{\uparrow_1 \downarrow_2} = \frac{1}{\sqrt{2}}\ket{1 \; 0} + \frac{1}{\sqrt{2}}\ket{0 \; 0} \end{gather}$$
$$\begin{gather} \ket{\downarrow_1 \uparrow_2} = \frac{1}{\sqrt{2}}\ket{1 \; 0} - \frac{1}{\sqrt{2}}\ket{0 \; 0} \end{gather}$$

Summing:
$$\begin{gather} \ket{1 \; 0} = \frac{1}{\sqrt{2}}[\ket{\uparrow_1 \downarrow_2} + \ket{\downarrow_1 \uparrow_2}] \end{gather}$$
Taking the difference:
$$\begin{gather} \ket{0 \; 0} = \frac{1}{\sqrt{2}} [\ket{\uparrow_1 \downarrow_2} -\ket{\downarrow_1 \uparrow_2}] \end{gather}$$
Where the spin matrices are defined as:
$$\begin{gather} \uparrow = \begin{bmatrix} 1 \\ 0 \end{bmatrix} \\ \downarrow = \begin{bmatrix} 0 \\ 1 \end{bmatrix}
\end{gather}$$

If we wanted to rotate our doublets (defined above):

$$\begin{gather} \chi' = u \chi \\ u = e^{\frac{1}{2}i\theta\hat n \times\tau}\end{gather}$$

Where $u$ is a rotation matrix, and $\tau$ is the Pauli spin matrices:

$$\begin{gather} \sigma_x = \begin{bmatrix} 0 & 1 \\ 1& 0 \end{bmatrix} \\ \sigma_y = \begin{bmatrix} 0 & i \\ -i & 0 \end{bmatrix} \\ \sigma_x = \begin{bmatrix} 1 & 0 \\ 0& -1 \end{bmatrix}\end{gather}$$
Example: for $\hat n = \hat y$: 

$$\begin{gather} u = \begin{bmatrix} \cos(\theta/2) & \sin(\theta/2) \\ -\sin(\theta/2) & \cos(\theta/2) \end{bmatrix} \end{gather}$$


## Orbital Angular Momentum
$L = 0,1,2,3,...$  $S,P,D,F,G,...$ 
$$\begin{gather} ^{2s+1}L_J \\ L = 0& S= 0 & J = 0  & ^1S_0 \\ L = 0 & S=1 & J=1 & ^3S_1 \\ L = 1 & S = 0 & J = 1 & ^1P_1 \\ L = 1 & S = 1 & J = 0,1,2 & ^3P_0, ^3P_1, ^3P_2 \\ L =2 & S= 0 & J =2 & ^1D_2 \\ L=2 & S=1 & J=1,2,3 & ^3D_1,\; ^3D_2\; ^3D_3\end{gather}$$
## Conserved Quantum Numbers under Strong interaction
$J$ - momentum, $Q$ - charge, $P$ - parity, $C$ Charge - conjugation (particle $\leftrightarrow$ anti-particle)

Parity $\vec{r} \to -\vec{r}$  $q \bar{q} \leftarrow (-1)$ 

Consider a wavefunction:

$$\begin{gather} P \psi(r) = \psi(-\vec{r}) = \eta_p \psi(r) \\ \psi(\vec{r}) = R(r) Y_{lm}(\theta, \phi) \\ \psi(-\vec{r}) = R(r)Y_{lm}(\pi-\theta,\pi+\phi) = R(r)(-1)^LY_{Lm}(\theta,\phi)\end{gather}$$

$P = -(-1)^L$
### Charge conjugation $C$ 
$$\begin{gather}\psi(\vec{r},\vec{s}) = R(r)Y_{Lm}(\theta,\phi) \chi(\vec{s}) \\ q \to \bar{q} \\ \bar{q} \to q \\ \vec{r} \to -\vec{r} \to (-1)^L \end{gather}$$ 
For spin: treat bosons and fermions differently
fermion and anti-fermion