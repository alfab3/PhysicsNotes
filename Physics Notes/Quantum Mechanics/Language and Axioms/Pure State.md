A Pure [[Quantum State]] is a state that can not be written as a probabilistic mixture of other quantum states.

A [[Density Matrix]] represents a pure state if and only if:

It can be written as an [[Outer Product]] of a [[State Vector]] with itself: 

$$\begin{gather} \rho= \ket{\psi}\bra{\psi} \end{gather}$$
It is a [[Projection]], in particular of [[Rank]] one

It is idempotent 

$$\begin{gather} \rho^2 = \rho \end{gather}$$
it has purity one: 

$$\begin{gather} \text{Tr}(\rho^2) = 1 \end{gather}$$

It is important to emphasize the difference between a probabilistic mixture of quantum states and their [[Quantum Superposition]]. If a physical system is prepared to be either in state $\ket{\psi_1}$ or $\ket{\psi_2}$, with equal probability it can be described by the mixed state: 

$$\begin{gather} \rho = \frac{1}{2}\begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} \end{gather}$$