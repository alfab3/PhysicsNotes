A class of [[Operators (Quantum Mechanics)]] that often play an important physical role is defined by those that correspond to a [[Change of Basis]], while keeping the new basis as an [[Orthonormal Basis]]. A common [[Unitary]] operator is the evolution operator, $U = e^{-iHt/\hbar}$ which enacts translation in time. Consider two sets of [[Basis]] states $\ket{i}$ and $\ket{i'}$ , related by a transformation operator $\mathcal R$ 

$$\begin{gather} \ket{i'} = \sum_i R_{i'i}\ket{i} \\ \bra{i'} = \sum_iR^*_{i'i}\bra{i} = \sum_i\bra{i}R^\dagger_{ii'}\end{gather}$$

$\ket{i'}$ states will refer to a new basis. The coefficients $\mathcal R_{i',i}$ must be constructed to retain the orthonormal properties:

$$\begin{gather} \braket{i'|j'} = \delta_{i'j'} \\ = \sum_{ij} R^\dagger_{ii'}R_{j'j} \braket{i|j} \\ = \sum_i R_{j'i}R^\dagger_{ii} \\ = (RR^\dagger)_{j'i'} \end{gather}$$

The Hermitian Conjugate of a [[Unitary]] Matrix is its inverse: i.e. $\mathcal R \mathcal R^\dagger = \mathbb I$ or equivalently: $\mathcal R^{-1} = R^\dagger$. An operator that satisfies this condition is called unitary. The word unitary follows from the fact that a state $U\ket{\psi}$ has the same [[Norm]] as $\ket{\psi}$, implying that the net probability is unchanged by the unitary transformation $U$. 
Hermitian operators are often used to generate unitary transformations: 

$$\begin{gather} U = e^{-i\mathcal K \theta} \\ \text{if } \mathcal K = \mathcal K^\dagger \\ UU^\dagger = e^{-i\mathcal K \theta}e^{i\mathcal K^\dagger \theta} = \mathbb I \end{gather}$$

Summarizing:


$$\begin{gather} U^\dagger = U^{-1} \\ \ket{\psi'} = U \ket{\psi} \\ \bra{\psi'} = \bra{\psi} U^\dagger \\ \mathcal A' = U \mathcal A U^\dagger \\ \braket{\psi'|\mathcal A' |\psi'} = \braket{\psi|\mathcal A |\psi} \end{gather}$$
