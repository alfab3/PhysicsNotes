## Schrodinger Representation
States evolve ([[Evolution in Time]]) while [[Operator]]s are fixed. The operators are sometimes labeled: 

$$\begin{gather} A_s(t) = A\end{gather}$$
## Heisenberg Representation
[[States]] are fixed, and the operators evolve in time. The time development of the operators can be expressed as a differential equation, where the rate of change of the operator is given by the commutation of the Hamiltonian with $A_s$ 

$$\begin{gather} A_H(t) = U^\dagger(t)A_sU(t) \\ \frac{d}{dt}A_H(t) =\frac{\partial}{\partial t}[U^\dagger(t) A_s(t) U(t)] \\ = \frac{i}{\hbar} U^\dagger[H(t),A_s(t)]U(t)+U^\dagger(t)\left(\frac{\partial}{\partial t} A_s(t)\right)U(t)\end{gather}$$
Where subscripts $S$ and $H$ refer to Schrodinger and Heisenberg representations respectfully.



## Hermitian Operators
If two [[Hermitian]] [[Operator]]s $\mathcal A$ and $\mathcal B$ commute, a set of [[States]] can be found that are eigenstates of both $\mathcal A$ and $\mathcal B$. To see this, consider eigenstates of $\mathcal B$: 

$$\begin{gather} \mathcal B\ket{b} = b\ket{b} \end{gather}$$

If $\mathcal A$ and $\mathcal B$ commute:

$$\begin{gather} \braket{b'|[\mathcal A, \mathcal B]|b} = 0 = (b-b')\braket{b'|\mathcal A|b} \end{gather}$$

This, the operator $\mathcal A$ does not mix states with different eigenvalues of $\mathcal B$. Or in other words, one can take the subset of states which have a given eigenvalue $b$, and this set should provide a basis for simultaneously diagonalizing $\mathcal A$.

This implies that any operator that commutes with the Hamiltonian is a constant of motion.