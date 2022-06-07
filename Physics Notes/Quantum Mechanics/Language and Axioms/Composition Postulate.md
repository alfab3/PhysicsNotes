The composition postulate deals with the structure of the [[Hilbert Space]] space of a composite system consisting of two or more subsystems. The postulate is naturally formulated for the case of two subsystems, and then straightforwardly generalized (by induction) to the case of many subsystems. 

The composition postulate states that the Hilbert space of a system consisting of two subsystems is a direct product of corresponding two Hilbert spaces. This, in particular, means that, if $\{e_n^{(I)}\}$ and $\{e_n^{(II)}\}$ are ONBs [[Orthonormal Basis]] in the Hilbert spaces of the systems $I$ and $II$, respectively, then the set of all vectors $$\begin{gather} \ket{e_{nm}} =\ket{e_n^{(I)}}\ket{e_n^{(II)}}, & \braket{e_{n_1m_1}|e_{n_2m_2}}=\delta_{n_1n_2}\delta_{m_1m_2}\end{gather}$$

forms thee basis in the Hilbert space of the composite system, so that a vector of state in this space can be represented as the following [[Linear Combination]]

$$\begin{gather} \ket{\psi} = \sum_{nm}c_{nm}\ket{e_{nm}} \equiv \sum_{nm} c_{nm}\ket{e_n^{(I)}}\ket{e_m^{(II)}}\end{gather}$$

Any linear operator acting in our Hilbert space can be represented as a linear combination of "elementary" composite operators of the following structure 

$$\begin{gather} O=A^{(I)}B^{(II)} \end{gather}$$

where the operator $A^{(I)}$ is a certain operator acting in the Hilbert space of subsystem $I$, and $B^{(II)}$ is a certain operator acting in the Hilbert space of subsystem $II$;  the action $O$ being described by the formula: 

$$\begin{gather} O\ket{\psi} = \sum_{nm}c_{nm}O\ket{e_{nm}} \equiv \sum_{nm} c_{nm}\ket{A^{(I)}e_n^{(I)}} \ket{B^{(II)}e_m^{(II)}} \end{gather}$$

An important special case of such an operator is when either $A^{(I)}$ or $B^{(II)}$ is a unity (a.k.a. identity) operator in its space; here we will use a shorthand notation:

$$\begin{gather} A^{(I)}\hat 1^{(II)} \equiv A^{(I)}, & \hat 1^{(I)}B^{(II)} \equiv B^{(II)}\end{gather}$$

Depending on the structure of the Hamiltonian, the two systems either interact with each other or not. The two subsystems do not interact with each other if and only if the composite system reduces to a direct sum of two independent Hamiltonians, each of the two dealing with corresponding subsystem:

$$\begin{gather} H = H^{(I)}+H^{(II)} \end{gather}$$

## Entanglement
A distinctively different from the issue of interaction is the notion of entanglement between the two subsystems. The notion of entanglement applies to the [[Density Matrix]] of the composite system. The two subsystems are called disentangled (with respect to each other) if the [[Density Matrix]] $\hat \rho$ of their composite state reduces to a direct product of individual density matrices: 

$$\begin{gather} \hat \rho = \hat \rho^{(I)}\hat \rho^{II}\end{gather}$$ 

If two subsystems are non-interacting and disentangled in the initial state, then the equation of motion: 
$$\begin{gather} i\hbar\frac{\partial}{\partial t}\hat \rho= H\hat\rho-\hat\rho H \equiv[H,\hat\rho] \end{gather}$$

or equivalently, the evolution equation: 

$$\begin{gather} \hat\rho(t) = U(t)\hat\rho(0)[U(t)]^\dagger \end{gather}$$

readily implies that the two subsystems are disentangled, with individual density matrices evolving in accordance with individual Hamiltonians.

Interaction leads to entanglement, by which we mean a structure of $\hat \rho$ that cannot be reduced to: $\hat \rho = \hat \rho^{(I)}\hat \rho^{II}$. As opposed to interaction which can vanish at a certain point of evolution, the entanglement if created will persist. Physically, the entanglement implies certain correlations between results of measurements dealing with the observables of both systems.

## Reduced density matrix
If we perform a measurement dealing with the observables of only one of the subsystems (subsystem $I$, for definiteness), then from the measurement postulate it follows that the outcome of this measurement is exhaustively described by the density matrix of the subsystem, related to the total density matrix by tracing out the variables of the other subsystem (note that the result of doing the trace is still an operator not a number):
$$\begin{gather}\hat \rho^{(I)} = \text{Tr}^{(II)} \hat \rho \equiv \sum_m\braket{e^{(II)}|\hat \rho|e^{(II)}}\end{gather}$$

In the matrix form,

$$\begin{gather} \rho^{(I)}_{n_1n_2} = \sum_m \rho_{n_1m;n_2m} & \rho_{n_1m;n_2m} = \braket{e_{n_1m_1}|\hat \rho|e_{n_2m_2}} \end{gather}$$

The operator $\hat \rho^{(I)}$ is called reduced density matrix of subsystem $I$. 

Quite often (but by no means always!), measuring an observable of the system $I$ leads to disentanglement upon measurement is that the observed eigenvalue is nondegenerate. In this case, the state of the systems disentangles into a product of corresponding pure state $\ket{\psi^{(I)}}$ of the system $I$ and a certain new state of the system $II$: 

$$\begin{gather}\hat\rho = \ket{\psi^{(I)}}\bra{\psi^{(I)}}\hat \rho^{(II)}_{\text{new}} \end{gather}$$

A bit less obvious is the fact that a measurement can also create an entangled state out of any state, including a disentangled one. All we need is that the eigenstates of the operator of corresponding observables are entangled states. 