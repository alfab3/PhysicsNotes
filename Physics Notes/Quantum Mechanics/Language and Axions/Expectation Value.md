## Definition
In [[Quantum Mechanics]] the expectation value is the probabilistic expected value of the result (measurement) of an experiment. It can be thought of as an average of all the possible outcomes of a measurement as weighted by their likelihood, and as such it is not the most probable value of a measurement; indeed the expectation value may have zero probability of occurring (e.g. measurements which can only yield integer values may have a non-integer mean).

Consider an [[Operator]] $A$. The expectation value is then $\braket{A} = \braket{\psi|A|\psi}$ in [[Dirac Notation]] with $\ket{\psi}$ a normalized [[State Vector]]. 

## Formalism
In quantum theory, an experimental setup is described by the observable $A$ to be measured, and the state $\sigma$ of the system. The expectation value of $A$ in the state $\sigma$ is denoted $\braket{A}_\sigma$.

Mathematically $A$ is a [[Self-Adjoint Operator]] on a [[Hilbert Space]]. In the most commonly used case in quantum mechanics $\sigma$ is a [[Pure State]], described by a normalized vector $\psi$ in Hilbert Space. The expectation value of $A$ in the state $\psi$ is defined as $$\begin{gather} \braket{A}_\psi = \braket{\psi|A|\psi} \end{gather}$$

If dynamics is considered, either the vector $\psi$ or the operator $A$ is taken to be time-dependent, depending on whether the [[Schrodinger Picture]] or [[Heisenberg Picture]] is used.

Given the probabilistic character of the measurement, it is often useful to address its statistical properties: the [[Expectation Value]]

$$\begin{gather} \bar {A} \equiv \braket{A}=\sum_\lambda \lambda p_\lambda & (\text{definition}) \end{gather}$$

and the [[Variance]]
$$\begin{gather} (\Delta A)^2 = \sum_\lambda(\lambda - \bar A)^2 p_\lambda & (\text{definition})\end{gather}$$

We now can find: 
$$\begin{gather}\bar A = \text{Tr}A\hat\rho & (\Delta A)^2 = \text{Tr}(A-\bar A)^2\hat \rho\end{gather}$$

For a pure state we have: 

$$\begin{gather}\bar A = \braket{\psi|A|\psi}, & (\Delta A)^2 =\braket{\psi|(A-\bar A)^2|\psi}\end{gather}$$