## Composition Postulate
The composition postulate states that the Hilbert space of a system consisting of two subsystems is a direct product of corresponding two Hilbert Spaces. If we have the set of Vectors: $\{\ket{e_n^{(I)}}\}$ and $\{\ket{e_n^{(II)}}\}$ which are ONBs in the Hilbert spaces of the systems $I$ and $II$ 

$$\begin{gather} \ket{e_{nm}}=\ket{e_n^{(I)}}\ket{e_m^{(II)}} & \braket{e_{n_1m_1}|e_{n_2m_2}}=\delta_{n_1n_2}\delta_{m_1m_2}\end{gather}$$
The state vector then takes the form: 
$$\begin{gather} \ket{\psi} = \sum_{nm}c_{nm}\ket{e_{nm}}\equiv \sum_{nm} c_{nm}\ket{e_n^{(I)}}\ket{e_m^{(II)}} \end{gather}$$
A linear operator acting in our Hilbert space can be represented as a linear combination of elementary composite operators of the following structure

$$\begin{gather} O = A^{(I)}B^{(II)} \end{gather}$$
Working with just one system implies the following:

$$\begin{gather} A^{(I)}\hat 1^{(II)} \equiv A^{(I)}, \hat 1B^{(II)} \equiv B^{(II)} \end{gather}$$
Applying this operator to our state results in the following:

$$\begin{gather} O\ket{\psi} =\sum_{nm}c_{nm}O\ket{e_{nm}}\equiv \sum_{nm}c_{nm}\ket{A^{(I)}e_n^{(I)}}\ket{B^{(II)}e_m^{(II)}} \end{gather}$$
Non-interacting subsystems:
$$\begin{gather} H = H^{(I)}+H^{(II)} \end{gather}$$

### Entanglement
A disentangled subsystem has composite density matrix: 
$$\begin{gather} \hat\rho = \hat \rho^{(I)} \hat\rho^{(II)} \end{gather}$$

### Reduced Density Matrix
With a composite system we can find the reduced density matrix of a single subsystem by tracing out the variables of the other subsystem:
$$\begin{gather}\hat\rho^{(I)} = \text{Tr}^{(II)}\hat \rho = \sum_m\braket{e_m^{(II)}|\hat\rho|e_m^{(II)}} \end{gather}$$
### Schmidt Decomposition
A special choice of orthonormal sets can be written as: 

$$\begin{gather} \ket{\psi} = \sum_n a_n \ket{\phi_n^{(I)}}\ket{\phi_n^{(II)}} \end{gather}$$
The reduced density matrix:
$$\begin{gather} \hat \rho^{(I)} = \sum_n|a_n|^2\ket{\phi_n^{(I)}}\bra{\phi_n^{(I)}} & \hat \rho^{(I)} = \sum_n|a_n|^2\ket{\phi_n^{(II)}}\bra{\phi_n^{(II)}} \end{gather}$$
