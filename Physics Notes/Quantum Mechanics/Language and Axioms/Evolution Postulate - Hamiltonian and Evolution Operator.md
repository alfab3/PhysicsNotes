The dynamic postulate of Quantum Mechanics states that the time evolution of the [[Density Matrix]] of an isolated system is prescribed by a certain [[Hermitian Operator]] $H$ called the system's [[Hamiltonian (QM)]] and acting in that system's [[Hilbert Space]] in accordance with the following equation of motion: 

$$\begin{gather} i\hbar\frac{\partial}{\partial t}\hat \rho= H\hat\rho-\hat\rho H \equiv[H,\hat\rho] \end{gather}$$

This equation is consistent with 
$$\begin{gather} \text{Tr} \hat \rho \equiv \sum_n \braket{e_n | \hat \rho | e_n} \equiv \sum_n \rho_{nn} =1 \end{gather}$$

Moreover, it preserves all the [[Eigenvalues]] (but not the [[Eigenvectors]]) of $\hat \rho$. Both statements are immediately implied by the following result: 

$$\begin{gather} \hat\rho(t) = \sum_j w_j\ket{\psi_j(t)}\bra{\psi_j(t)}\end{gather}$$

where $\ket{\psi_j(t)}$ evolves in accordance with the [[Schrodinger Equation]] for a [[Pure State]]

$$\begin{gather} i\hbar\frac{\partial}{\partial t}\ket{\psi_j(t)}=H\ket{\psi_j(t)} \end{gather}$$

With the above two equations  we see that the interpretation of $\hat \rho$ ([[Density Matrix]]) as a statistical mixture of pure states applies not only to an instant state, but to the whole process of evolution of $\hat \rho$. Each of the [[Eigenstate]]s $\ket{\psi_j(t)}$ evolves individually in accordance with Schrodinger's equation, the probabilities $w_j$ remaining intact. 

The relationship with the Schrodinger equation allows us to invoke the [[Evolution Operator]], $U(t)$ 

$$\begin{gather} \ket{\psi_j(t)} = U(t)\ket{\psi_j(0)}, & \bra{\psi_j(t)} = \bra{\psi_j(0)}[U(t)]^\dagger \end{gather}$$

Combining these with our definition of $\hat \rho(t)$ we can see that:

$$\begin{gather} \hat\rho(t) = U(t)\hat\rho(0)[U(t)]^\dagger \end{gather}$$

### Time-independent Hamiltonian

Along with the representation for $\hat \rho$ in terms of its [[Eigenvectors]], yet another very important representation in the case of time-independent [[Hamiltonian (QM)]] is in terms of the Hamiltonian (i.e. energy) [[Eigenstate]]s $\{\ket{n}\}$,

$$\begin{gather} H\ket{n}=E_n\ket{n} \end{gather}$$

Starting from the state vector with the evolution operator and taking into account that for a time-independent Hamiltonian we have: 

$$\begin{gather} U(t)=e^{-iHt/\hbar} \end{gather}$$

for the matrix $\rho_{nm}(t) = \braket{n|\hat \rho(t)|m}$ we readily get

$$\begin{gather} \rho_{nm}(t)=\rho_{nm}(0)e^{it(E_m-E_n)/\hbar} \end{gather}$$

This formula is especially important for the discussion of the relaxation in an isolated system. If, after a long enough time of system's evolution, we completely lose control on the value of the phases $t(E_m-E_n)/\hbar$ modulo $2\pi$, then, for all practical purposes we should replace our actual [[Density Matrix]] with the one averaged over the values of the phases $t(E_m-E_n)/\hbar$. This amounts to vanishing the off-diagonal terms:

$$\begin{gather} \rho_{nm}(t) \rightarrow \delta_{nm}\rho_{nn}(0) \end{gather}$$

meaning that our state is indistinguishable from a statistical mixture of energy eigenstates, the state $\ket{n}$ entering the ensemble with the probability $\rho_{nn}(0)$