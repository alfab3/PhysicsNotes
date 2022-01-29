The dynamic postulate of Quantum Mechanics states that the time evolution of the [[Density Matrix]] of an isolated system is prescribed by a certain [[Hermitian Operator]] $H$ called the system's [[Hamiltonian (QM)]] and acting in that system's [[Hilbert Space]] in accordance with the following equation of motion: 

$$\begin{gather} i\hbar\frac{\partial}{\partial t}\hat \rho= H\hat\rho-\hat\rho H \equiv[H,\hat\rho] \end{gather}$$

This equation is consistent with 
$$\begin{gather} \text{Tr} \hat \rho \equiv \sum_n \braket{e_n | \hat \rho | e_n} \equiv \sum_n \rho_{nn} =1 \end{gather}$$

Moreover, it preserves all the [[Eigenvalues]] (but not the [[Eigenvectors]]) of $\hat \rho$. Both statements are immediately implied by the following result: 

$$\begin{gather} \hat\rho(t) = \sum_j w_j\ket{\psi_j(t)}\bra{\psi_j(t)}\end{gather}$$

where $\ket{\psi_j(t)}$ evolves in accordance with the [[Schrodinger Equation]] for a [[Pure State]]

$$\begin{gather} i\hbar\frac{\partial}{\partial t}\ket{\psi_j(t)}=H\ket{\psi_j(t)} \end{gather}$$