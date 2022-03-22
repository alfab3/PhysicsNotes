## Definition of 2-Level Hamiltonian
Let $\ket{e_1}$ and $\ket{e_2}$ be some ONB ([[Orthonormal Basis]]) in our two-dimensional Hilbert space, so that a pure state in our space is represented as 

$$\begin{gather} \ket{\psi} = \alpha\ket{e_1} + \beta\ket{e_2} = \begin{bmatrix} \alpha \\ \beta \end{bmatrix}\end{gather}$$
With the selected ONB, any operator, including the most general [[Hamiltonian]] is represented as a matrix: 



$$\begin{gather} \hat H = \begin{bmatrix} H_{11} & H_{12} \\ H_{21} & H_{22} \end{bmatrix} \end{gather}$$


(Note: since $\hat H$ is Hermitian ([[Hermitian]]) $H_{12} = \overline{H_{21}}$, the off-diagonal element is called "a mixing matrix element") We parameterize $H_{12} = -\Delta e^{i\varphi}$. 

## $\Delta = 0$ 
A simple case if $\Delta = 0$ then our basis and Hamiltonian [[Eigenstate]]s coincide: 


$$\begin{gather} \begin{bmatrix} H_{11} & 0 \\ 0 & H_{22} \end{bmatrix} \begin{bmatrix} 1 \\ 0\end{bmatrix} = H_{11} \begin{bmatrix} 1 \\ 0\end{bmatrix} = E_1 \ket{e_1} & (E_1 = H_{11})\\\begin{bmatrix} H_{11} & 0 \\ 0 & H_{22} \end{bmatrix} \begin{bmatrix} 0 \\ 1\end{bmatrix} = H_{22} \begin{bmatrix} 0 \\ 1\end{bmatrix} = E_2 \ket{e_2} & (E_2 = H_{22})\end{gather}$$
## Generic Parameterization
The absolute value of energy is not observable - it can be shifted by an arbitrary constant $E_0$ without any effect on quantum-mechanical observables. 

The generic parameterization of the Hamiltonian can be written as:

$$\begin{gather} \hat H = \begin{bmatrix} \xi & -\Delta e^{i\varphi} \\ -\Delta e^{-i\varphi} & \xi \end{bmatrix} \end{gather}$$

## Dynamics
The dynamics of the system are governed by the [[Schrodinger Equation]]:


$$\begin{gather} i\hbar \frac{\partial}{\partial t}\ket{\psi} = \hat H\ket{\psi} & \Leftrightarrow & i\hbar \begin{bmatrix} \dot \alpha \\ \dot \beta \end{bmatrix} = \begin{bmatrix} \xi & -\Delta e^{i\varphi} \\ -\Delta e^{-i\varphi} & \xi \end{bmatrix} \begin{bmatrix} \dot \alpha \\ \dot \beta \end{bmatrix}\end{gather}$$

Solving for the eigenvalues gives us: 

$$\begin{gather} E_{\pm} = \pm \epsilon & \epsilon = \sqrt{\xi^2 + \Delta^2}\end{gather}$$
And corresponding eigenvectors: 
$$\begin{gather} \ket{-} = \begin{bmatrix} \alpha_- \\ \beta_- \end{bmatrix} = \begin{bmatrix} e^{i\varphi} \sin\theta \\ \cos \theta  \end{bmatrix} & \ket{+} = \begin{bmatrix} \alpha_+ \\ \beta_+ \end{bmatrix} = \begin{bmatrix} e^{i\varphi} \cos\theta \\ -\sin \theta  \end{bmatrix} \end{gather}$$

For the mixing angle: 

$$\begin{gather} \theta=\tan^{-1}\frac{\Delta}{\xi + \epsilon} & \cos\theta = \frac{\sqrt{1+\xi/\epsilon}}{\sqrt {2}} & \sin \theta =\frac{\sqrt{1-\xi/\epsilon}}{\sqrt{2}} \end{gather}$$

The solution of the [[Schrodinger Equation]] then reads (setting $\hbar = 1$) 

$$\begin{gather} \ket{\psi(t)} = \braket{+| \psi(0)} e^{-i\epsilon t}\ket{+} + \braket{-| \psi(0)} e^{i\epsilon t}\ket{-} \end{gather}$$


## Special Case of $\ket{\psi_1} = \ket{e_1}$ 
There is actually nothing special about this initial condition, because any state can be selected to be a basis state. 

Our first case:


$$\begin{gather} \ket{\psi_1(t)} = \alpha_+^*e^{-i\epsilon t} \begin{bmatrix} \alpha_+ \\ \beta_+\end{bmatrix} + a^*_-e^{i\epsilon t} \begin{bmatrix} \alpha_- \\ \beta_-\end{bmatrix} = e^{-i\epsilon t} \begin{bmatrix} |\alpha_+|^2 \\ \beta_+\end{bmatrix} + e^{i\epsilon t} \begin{bmatrix} |\alpha_-|^2 \\ \beta_-\end{bmatrix} \end{gather}$$

This defines the probability amplitude of finding the system in state $\ket{e_1}$ at time $t$ if it was in the state $\ket{e_1}$ at $t=0$:

$$\begin{gather} A_{11} = \braket{e_1|\psi_1(t)} = \cos(\epsilon t) - i\frac{\xi}{\epsilon}\sin(\epsilon t) \end{gather}$$

The probability itself is: 

$$\begin{gather}P_{11} = |A_{11}|^2 \equiv 1 - \frac{\Delta^2}{\epsilon^2}\sin^2(\epsilon t)\end{gather}$$
The same process can be done for $\ket{\psi_2}$ 
$$\begin{gather} A_{22} = \braket{e_2|\psi_2(t)} = \cos(\epsilon t) + i\frac{\xi}{\epsilon}\sin(\epsilon t) \end{gather}$$and: 
$$\begin{gather}P_{22} = |A_{22}|^2 \equiv 1 - \frac{\Delta^2}{\epsilon^2}\sin^2(\epsilon t)\end{gather}$$

For the complimentary probabilities: 

$$\begin{gather} P_{21} = |\braket{e_2|\psi_1(t)}|^2 = 1 - P_{11} = \frac{\Delta^2}{\epsilon^2} \sin^2(\epsilon t) \end{gather}$$
