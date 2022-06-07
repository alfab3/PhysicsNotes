## Definition
For any finite system, states are discrete and can be assigned labels. The discrete nature of states is what is meant by the word "quantized." Foe some systems the number of such discrete states is finite, e.g. a particle in either spin up or spin down state, whereas in other systems the number of states are infinite, e.g. levels of a [[Quantum Harmonic Oscillator]]. 

Any physical state can be assigned a label, in this case $\psi$. This state can always be expressed as a [[Linear Combination]] of basis states, $\ket{i}$, in an [[Orthonormal Basis]]. These states can be expressed as vectors in a vector space of size $n$:

$$\begin{gather} \ket{1} = \hat{1} = \begin{bmatrix} 1 \\ 0 \\ 0 \\ \vdots \\ 0 \end{bmatrix}, \; \ket{2} = \hat{2} = \begin{bmatrix} 0 \\ 1 \\ 0 \\ \vdots \\ 0 \end{bmatrix}, \; \ket{n} = \hat{n} = \begin{bmatrix} 0 \\ 0 \\ 0 \\ \vdots \\ 1 \end{bmatrix}   \end{gather}$$
The basis is orthonormal: $$\begin{gather} \braket{i|j} = \hat i^* \cdot \hat j = \delta_{ij}\end{gather}$$
See: [[Dirac Notation]]

States are formed by taking linear combinations of basis states $\ket{i}$: 

$$\begin{gather} \ket{\psi} = \sum_i a_{\psi,i} \ket{i} \\ \bra{\psi} = \sum_i a_{\psi,i}^* \bra{i}\end{gather}$$

Where $a_{i,\psi}$ is a complex number. By taking the overlap of $\ket{\psi}$ with $\bra{i}$, one sees that 

$$\begin{gather} a_{i,\psi} = \braket{i|\psi} \end{gather}$$

Norm: 

$$\begin{gather} \braket{\psi|\psi} = \sum_i \braket{\psi|i}\braket{i|\psi} \\ = \sum_i|\braket{\psi|i}|^2 = \sum_i|a_{\psi,i}|^2 \end{gather}$$

If the state $\ket{\psi}$ is normalized, i.e. $\braket{\psi|\psi} = 1 = \sum_i|\braket{i|\psi}|^2 = \sum_i |a_{\psi,i}|^2$ the squared element $|\braket{i|\psi}|^2$ can be interpreted as a probability because each term is positive and because the sum yields unity. Thus, if one prepares a state $\ket{\psi}$, the chance one finds that one is in a state $\ket{i}$ is $|\braket{i|\psi}|^2$.

Completeness relation: $$\begin{gather} \sum_i \ket{i} \bra{i} = \mathbb I \end{gather}$$ 