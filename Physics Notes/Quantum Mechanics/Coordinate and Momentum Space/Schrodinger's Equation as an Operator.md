Before we find solutions, we regress to consider the notation and vocabulary associated with the [[Schrodinger Equation]]. One often writes the [[Hamiltonian]] in this way: 

$$\begin{gather} H\psi(x) = E\psi(x), & H = -\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2} + V(x) \end{gather}$$

Referring to $H$ above as the Hamiltonian is actually incorrect, as it does not represent the fact that the Hamiltonian is an operator and should be sandwiched between a bra and ket. Operators are defined by matrix elements, and should referenced by two labels. In this case $\braket{x'|H|x}$ which should be considered a function of both $x$ and $x'$. More correctly, beginning with $H$ defined as an operator, then using completeness, $$\begin{gather} H \ket{\psi} = E\ket{\psi} \\ \int dx' \braket{x|H|x'}\braket{x'|\psi} = E\braket{x|\psi} \end{gather}$$
Now one assumes that $H$ does not mix $\ket{x}$ with $\ket{x'}$ unless $x$ and $x'$ are a the same position(or neighboring positions in the limit that one discretizes coordinate space). In that case one can define the function $h(x)$ as $$\begin{gather} \braket{x|H|x'} = h(x)\delta(x-x') \end{gather}$$ and Schrodinger's Equation becomes 

$$\begin{gather} h(x)\braket{x|\psi}=E\braket{x|\psi} \\ h(x)\psi(x) = E\psi(x) \\ h(x) = -\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}+V(x)\end{gather}$$
