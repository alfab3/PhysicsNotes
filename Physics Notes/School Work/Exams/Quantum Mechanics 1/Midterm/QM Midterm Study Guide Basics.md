## Bra-ket Notation
A ket is defined as:
$$\begin{gather} \ket{\psi} = \begin{bmatrix} n_1 \\ n_2 \\ n_3 \\ \vdots\\ n_j \end{bmatrix}  \end{gather}$$

A bra is defined as: 
$$\begin{gather} \bra{\psi} = [n^*_1 & n^*_2 & n^*_3 & \cdots & n^*_j] \end{gather}$$

## Trace
The trace of an $n \times n$ square matrix $A$ is defined as 
$$\begin{gather} \text{Tr}(A)=\sum^n_{i=1} a_{ii} = a_{11}+a_{22}+ \cdots + a_{nn} \end{gather}$$
#### Cyclic property:
$$\begin{gather} \text{Tr}(AB) = \text{Tr}(BA)\end{gather}$$
#### Bra-ket Notation:

$$\begin{gather} \text{Tr}\hat\rho = \sum_n \bra{e_n}\hat \rho\ket{e_n} \end{gather}$$


## System's Hilbert Space
A state vector is defined as: 
$$\begin{gather} \ket{\psi} = \sum_n c_n\ket{e_n} & c_n = \braket{e_n|\psi}\end{gather}$$

Where $\{\ket{e_n}\}$ is a certain orthonormal basis.

If the vector were instead defined as a bra:

$$\begin{gather} \bra{\psi} = \sum_n c^*_n\bra{e_n} & c_n = \braket{e_n|\psi}\end{gather}$$
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
The probability of finding $\lambda$ in the state: $\rho^{(new)}$ is defined by: 

$$\begin{gather} p_\lambda = \text{Tr}(\hat \rho \hat P_\lambda) \end{gather}$$
Where $\hat \rho^{(new)}$ is defined as:
$$\begin{gather} \hat\rho^{(new)} \frac{\hat P_\lambda \hat \rho \hat P_\lambda}{\text{Tr}\hat P_\lambda\hat\rho \hat P_\lambda} 
 = \frac{\hat P_\lambda \hat\rho\hat P_\lambda}{p_\lambda}\end{gather}$$
 ## Probability

### Pure State
 If the state $\hat \rho$ is pure $\hat \rho = \ket{\psi}\bra{\psi}$ and $\lambda$ is non-degenerate, the probability of finding $\lambda$ is: 
 $$\begin{gather} p_\lambda = |\braket{e_\lambda|\psi}|^2 \end{gather}$$
### Mixed State
If $\hat \rho$ is a mixed state the probability can be found by:
 $$\begin{gather} p_\lambda = \sum_j \sum_\nu w_j|\braket{e_{\lambda,\nu}|\psi}|^2 \end{gather}$$
## Expectation Value and Variance
Assume we have some observable $A$:

The expectation value can be found by: 

$$\begin{gather}\bar{A} \equiv \braket{A} = \sum_\lambda \lambda p_\lambda \\ \bar{A} = \text{Tr} A\hat{\rho} \\ (\Delta A^2) = \text{Tr}(A-\bar{A}^2)\hat \rho\end{gather}$$
Variance: 
$$\begin{gather} (\Delta A)^2 = \sum_\lambda (\lambda-\bar{A})^2p_\lambda \\ \bar{A} =\braket{\psi|A|\psi} \\ (\Delta A)^2 = \braket{\psi|(A-\bar{A})|\psi}\end{gather}$$
 ## Appendix 
 Degenerate/Non-degenerate - a degenerate eigenvalue is an eigenvalue which corresponds to multiple eigenvectors. 