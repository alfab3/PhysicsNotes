Consider two [[Hermitian Operator]]s $\mathcal A$ and $\mathcal B$. One can choose states to be [[Eigenstate]]s of either operator but not necessarily both. This depends on whether the two operators commute. If there existed a basis where all the basis [[States]] were eigenstates of both $\mathcal A$ and $\mathcal B$ one could state that

$$\begin{gather} \mathcal A \mathcal B\ket{ab} = ab \ket{ab} \\ \mathcal B \mathcal A \ket{ab} = ab\ket{ab} \end{gather}$$

In this case the products $\mathcal A \mathcal B$ and $\mathcal B \mathcal A$ would return the same result acting on any basis state and one could say $$\begin{gather} \mathcal A \mathcal B = \mathcal B \mathcal A \\ [\mathcal A, \mathcal B] = 0 \end{gather}$$

Thus, the commutation of operators is essential if one is to be able to find a basis that serves as eigenstates for both operators.

For the case where the operators no longer commute one can find an uncertainty relation. The non-commutation results in some non-zero operator $\mathcal C$ :

$$\begin{gather} [\mathcal A, \mathcal B] = i\mathcal C \end{gather}$$
The operator $\mathcal C$ must be [[Hermitian]] because the commutation of two Hermitian operators must be anti-Hermitian.

To derive the Uncertainty Relation, one begins with [[Cauchy-Schwarz Inequality]]

Leads to: 

$$\begin{gather} \braket{\psi|\delta X^2|\psi}\braket{\psi|\delta P^2|\psi} \geq \frac{\hbar^2}{4} \\ \delta \mathcal A \equiv \mathcal A-\braket{\psi|\mathcal A|\psi} \end{gather}$$