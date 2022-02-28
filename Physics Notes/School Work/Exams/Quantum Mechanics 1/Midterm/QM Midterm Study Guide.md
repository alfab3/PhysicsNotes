## System's Hilbert Space
A state vector is defined as: 
$$\begin{gather} \ket{\psi} = \sum_n c_n\ket{e_n} & c_n = \braket{e_n|\psi}\end{gather}$$

Where $\{\ket{e_n}\}$ is a certain orthonormal basis.

## Density Matrix
The state of the system is defined by a density matrix $\hat \rho$, a Hermitian Operator with non-negative eigenvalues and unity trace

$$\begin{gather} \text{Tr} \hat \rho \equiv \sum_n \braket{e_n | \hat \rho | e_n} \equiv \sum_n \rho_{nn} =1 \end{gather}$$
#### Pure state
A pure state $\ket{\psi}$ has a density matrix of the form:
$$\begin{gather} \hat \rho_\psi = \ket{\psi}\bra{\psi}, & \braket{\psi|\psi} = 1 & \text{(pure state)}\end{gather}$$

#### Mixed State
A mixed state can be interpreted as a statistical mixture of a special set of pure states. Namely a random choice with probability $w_j$ of one of the pure states $\{\ket{\psi_j}\}$, corresponding  to the eigenvectors of the density matrix: 
$$\begin{gather}\hat \rho \ket{\psi_j} = w_j\ket{\psi_j} \end{gather}$$
$$\begin{gather} \hat \rho = \sum_j w_j\ket{\psi_j}\bra{\psi_j} & \braket{\psi_{j_1}|\psi_{j_2}} = \delta_{j_1j_2}\end{gather}$$
## Projection Operator
Assume we have some eigenvalue $\lambda$

##### Non-degenerate
$$\begin{gather} \hat P_\lambda = \ket{e_\lambda}\bra{e_\lambda} \end{gather}$$
where $\ket{e_\lambda}$ is corresponding unit eigenvector of the operator $A$: $A\ket{e_\lambda} = \lambda \ket{e_\lambda}$ 

##### Degenerate 

$$\begin{gather} \hat{P}_\lambda = \sum_\nu \ket{e_{\lambda,\nu}} \bra{e_{\lambda,\nu}} \end{gather}$$

##### Properties
$$\begin{gather} A = \sum_\lambda \lambda \hat P_\lambda \\ \hat P_\lambda \hat P_{\lambda'} = \delta_{\lambda,\lambda'} \hat P_\lambda \\ \sum_\lambda \hat P_\lambda = \hat 1 & \text{completeness relation}\end{gather}$$

## Measuring Postulate
