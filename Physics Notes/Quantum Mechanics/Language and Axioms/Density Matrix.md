## Definition
We can define a state $\psi$ as a vector, or as a density matrix: 
$$\begin{gather} \rho_\psi = \ket{\psi}\bra{\psi} \\ (\rho_\psi)_{ij} = \psi_i\psi_j^* \end{gather}$$

The density matrix is [[Hermitian]]. From the definition of the density matrix, one can write the state $\ket{\psi}$ as a vector and the operator $\mathcal K$ as a matrix: 

$$\begin{gather} \braket{\psi|\mathcal K|\psi} = \sum_{ij} \psi^*_i\mathcal K_{ij} \psi_j = \text{Tr} (\rho _\psi \mathcal K)\\ |\braket{\phi|\mathcal K|\psi}|^2 = \text{Tr} \rho_\psi\mathcal K^\dagger \rho_\phi \mathcal Ks\end{gather}$$

Where "Tr" defines the [[Trace]] operation. 

The trace of any product of operators, or matrices, is invariant to unitary transformations.

For a state $\ket{\psi}$ with a basis: 

$$\begin{gather} \ket{\psi} = \begin{pmatrix} 1 \\ 0 \\ \vdots \\ 0 \end{pmatrix} \end{gather}$$

In this basis $\rho_\psi$ is diagonalized and has the form: 

$$\begin{gather} \rho_\psi = \begin{pmatrix} 1 & 0 & \ldots & 0 \\ 0  & 0 & \ldots & 0  \\ && \vdots \\ 0 & 0 & \ldots 0\end{pmatrix} \end{gather}$$
A density matrix that can be diagonalized in such a way is called a pure wstate.
## Projection Operator

A [[Projection Operator]] is a density matrix corresponding to a [[Pure State]]. 

Obeys: 

$$\begin{gather} P^2_\psi = P_\psi \\ \text{Tr}P_\psi = 1 \end{gather}$$
Example: $$\begin{gather} a\ket{\psi} + b\ket{\phi} \\ P_\psi \to a \ket{\psi} \end{gather}$$

A more general density matrix which is an incoherent sum over several states, the resulting diagonalized matrix could have more than one nonzero element. For instance we can define the following density matrix 

$$\begin{gather} \rho = \frac{1}{2} \ket{1}\bra{1} + \frac{1}{2}\ket{2}\bra{2} \end{gather}$$

The density matrix describes being in state $\ket{1}$ 50% of the time and in state $\ket{2}$ 50% of the time. 