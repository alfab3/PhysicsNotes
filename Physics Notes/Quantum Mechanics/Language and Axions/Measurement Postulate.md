Speaking generally the state of the system cannot be directly observed. Rather, $\hat \rho$ describes a two-fold probabilistic outcome of observation (aka measurement), as a result of which an observer 1) finds a certain distinct value of the quantity being "observed/measured" and 2) finds the new state of the system. It is a fundamental feature of Quantum Mechanics that, speaking generally, an observation changes the state of the system. The measurement axiom of Quantum Mechanics states that each measurement is described by corresponding [[Hermitian]] Operator. If the measurement deals with the operator $A$ (we say: "A is being measured"), then possible outcomes of the measurement correspond to a set $\{\lambda\}$ of real [[Eigenvalues]] of $A$, while the probability $p_\lambda$ of finding a particular value $\lambda$ and the new state $\hat \rho^{(new)}$, and the projector $\hat P_\lambda$ of the $\lambda$ [[Eigenspace]] of the operator $A$:

$$\begin{gather} p_\lambda = \text{Tr}\hat \rho \hat P _\lambda \\ \hat \rho^{(new)} = \frac{\hat P_\lambda\hat \rho\hat P_\lambda }{\text{Tr}\hat P_\lambda \hat \rho \hat P_\lambda} = \frac{\hat P _\lambda \hat \rho \hat P_\lambda}{p_\lambda}\end{gather}$$

The denominator here is merely a normalization constant making $\hat \rho$ consistent with the requirement: 

$$\begin{gather} \text{Tr}\hat \rho \equiv \sum_n \braket{e_n|\hat \rho|e_n} \equiv \sum_n \rho_{nn} =1 \end{gather}$$

Please see: [[Projection Operator]].

A particularly simple and important case of measurement corresponds to observation of a non-degenerate eigenvalue $\lambda$. Here $\hat \rho^{(new)}$ is necessarily a pure state exhaustively defined by observed $\lambda$:

$$\begin{gather}\hat \rho ^{(new)} = \hat P_\lambda = \ket{e_\lambda}\bra{e_\lambda} & (\text{non-degenerate }\lambda) \end{gather}$$

while the probability of observing $\lambda$ is given by a simple formula 

$$\begin{gather}p_\lambda = \braket{e_\lambda|\hat\rho|e_\lambda} & (\text{non-degenerate }\lambda)\end{gather}$$

This means that a pure state can be prepared by observing a non degenerate eigenvalue in the process of measurement, irrespective of the state before measurement.
Let us now look at some extra special cases. If the state $\hat \rho$ before measurement is pure, $\hat \rho = \ket{\psi}\bra{\psi}$, then the expression for the probability $p_\lambda$ further simplifies to 
$$\begin{gather} p_\lambda = |\braket{e_\lambda|\psi}|^2 & (\hat \rho = \ket{\psi}\bra{\psi} \text{ and nondegenerate} \lambda) \end{gather}$$

If the state $\hat \rho$ before measurement is pure, the new state is necessarily pure no matter whether the eigenvalue $\lambda$ is degenerate or not - and the following formulas apply 

$$\begin{gather} \hat \rho = \frac{1}{p_\lambda}\ket{\hat P_\lambda \psi}\bra{\hat P _\lambda\psi} & (\hat \rho = \ket{\psi}\bra{\psi}) \\ p_\lambda = \braket{\psi|\hat P_\lambda|\psi} = \braket{\hat P_\lambda|\hat P_\lambda \psi} & (\hat \rho = \ket{\psi}\bra{\psi}) \end{gather}$$

Here $\ket{\hat P_\lambda \psi} \equiv \hat P_\lambda\ket{\psi}$

Given the probabilistic character of the measurement, it is often useful to address its statistical properties: the [[Expectation Value]]

$$\begin{gather} \bar {A} \equiv \braket{A}=\sum_\lambda \lambda p_\lambda & (\text{definition}) \end{gather}$$

and the [[Variance]]
$$\begin{gather} (\Delta A)^2 = \sum_\lambda(\lambda - \bar A)^2 p_\lambda & (\text{definition})\end{gather}$$

We now can find: 
$$\begin{gather}\bar A = \text{Tr}A\hat\rho & (\Delta A)^2 = \text{Tr}(A-\bar A)^2\hat \rho\end{gather}$$

For a pure state we have: 

$$\begin{gather}\bar A = \braket{\psi|A|\psi}, & (\Delta A)^2 =\braket{\psi|(A-\bar A)^2|\psi}\end{gather}$$