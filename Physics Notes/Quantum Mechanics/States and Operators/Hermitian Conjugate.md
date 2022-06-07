Consider a matrix element $\braket{\phi|\mathcal A| \psi}$. Expressing the [[Operators (Quantum Mechanics)]] as matrices and the states as vectors then taking the [[Complex Conjugate]]:

$$\begin{gather} \braket{\phi|\mathcal A|\psi} = \phi_i^*a_{ij}\psi_j  \\ \braket{\phi|\mathcal A|\psi}^* = (\phi_i^*a_{ij}\psi_j)^* = \psi_j^* a^*_{ij} \phi_j \end{gather}$$

Thus if one wishes to define an operator $\mathcal A^\dagger$ such that:

$$\begin{gather} \braket{\psi|\mathcal A^\dagger | \phi} = \braket{\phi|\mathcal A| \psi}^* \end{gather}$$

for any states $\ket{\phi}$ and $\ket{\psi}$ the operator $\mathcal A^\dagger$ must be represented by the complex conjugate of the matrix that represents $\mathcal A$, then transposed. 

$$\begin{gather} \mathcal A^\dagger = \sum_{ij}(a^\dagger)_{ij}\ket{i}\bra{j} \\ (a^\dagger)_{ij} = a^*_{ji} \end{gather}$$
The operator $\mathcal A^\dagger$ is known as the Hermitian Conjugate of $\mathcal A$. A Hermitian operator is one that obeys the relation $\mathcal A = \mathcal A^\dagger$. The eigenvalues of a Hermitian operator are real, i.e. one can always find a [[Change of Basis]] that diagonalizes $\mathcal A$, with the elements all being real. To see this, assume the operator $\mathcal A$ has [[Eigenvalues]] $a_i$ and [[Eigenvectors]] $\ket{i}$. 

$$\begin{gather} \mathcal A\ket{i} = a_i\ket{i} \\ \bra{i} \mathcal A^\dagger = a^*_i\bra{i} \\ \braket{i|(\mathcal A-\mathcal A^\dagger)|i} = a_i - a^*_i \end{gather}$$

If $\mathcal A$ is Hermitian, $\mathcal A = \mathcal A^\dagger$, and $a_i$ must equal $a_i^*$ so the eigenvalues are real Hermitian operators are important for two reasons:

They yield real numbers as expectations, $\braket{\psi|\mathcal K|\psi}^* = \braket{\psi|\mathcal K |\psi}$. Because all physical observables are real, they need to be represented by Hermitian operators. An example is the Hamiltonian $H$ which represents the energy of a system. 

They can be used to generate [[Unitary Transformations]]: for example: $e^{iK\theta}$, An example is the time evolution operator $e^{-iHt}$. 