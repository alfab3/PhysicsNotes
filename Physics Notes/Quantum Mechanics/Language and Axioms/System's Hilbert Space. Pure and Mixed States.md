A quantum mechanical system is characterized by a complete [[Inner Product Spaces]] - that is, [[Hilbert Space]] - with either finite or countably infinite basis. This space is termed system's Hilbert Space. In the system's Hilbert space, each vector $\ket{\psi}$ (referred to as a vector of state aka pure state, aka wave function) can be represented as the following finite or countably infinite sum 

$$\begin{gather} \ket{\psi} = \sum_n c_n\ket{e_n}, & c_n = \braket{e_n|\psi} \end{gather}$$

where $\{\ket{e_n}\}$ is a certain [[Orthonormal Basis]] (ONB):

$$\begin{gather} \braket{e_{n_1}|e_{n_2}} = \delta_{n_1,n_2}\end{gather}$$

In the most general case, the state of the system is described by the so called density matrix (aka density operator), $\hat \rho$, a [[Hermitian]] operator with non-negative [[Eigenvalues]] and unity [[Trace]]

$$\begin{gather} \text{Tr} \hat \rho \equiv \sum_n \braket{e_n | \hat \rho | e_n} \equiv \sum_n \rho_{nn} =1 \end{gather}$$

A special class of states, the pure states, are associated with the (normalized to unity) vectors of states. By definition, the density matrix $\hat \rho_\psi$ of a pure state $\ket{\psi}$ has the form: 

$$\begin{gather} \hat \rho_\psi = \ket{\psi}\bra{\psi}, & \braket{\psi|\psi} = 1 & \text{(pure state)}\end{gather}$$

The states that are not pure states are called mixed states.