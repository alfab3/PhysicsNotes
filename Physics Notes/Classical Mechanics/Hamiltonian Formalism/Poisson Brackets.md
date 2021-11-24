Poisson Bracket, $\{A,B\}$ is a function of coordinates, momenta and speaking generally time constructed from the two other functions, $A(\{q,p\},t)$ and $B(\{q,p\},t)$ by the following rule:
$$\begin{gather}\{A,B\} = \sum_j\left[\frac{\partial A}{\partial p_j}\frac{\partial B}{\partial q_j} - \frac{\partial A}{\partial q_j}\frac{\partial B}{\partial p_j}\right] \end{gather}$$

where the sum is over all $j$'s. Note that $\{A,B\} = - \{B,A\}$, implying $\{A,A\} =0$ for any $A$. Clearly if both $A$ and $B$ do not explicitly depend on time, then $\{A,B\}$ is also free of explicit time dependence. 

For any function of coordinates, momenta, and time, $A(\{q,p\},t)$, its total time derivative during the evolution can be expressed as $$\begin{gather} \dot A \equiv \frac{d}{dt}A(\{q,p\},t) = \{H,A\} +\frac{\partial A}{\partial t} \end{gather}$$. In particular, if $A$ does not depend on time explicitly - which actually is the most typical case, then $$\begin{gather} \dot A = \{H,A\} \;\;\; [ A \equiv A(\{q,p\})]\end{gather}$$

Hence any quantity $A(\{q,p\})$ is a constant of motion if and only if, its Poisson bracket with the Hamiltonian([[Hamiltonian Function and Hamilton's Equations]]) is zero, no matter whether the Hamiltonian depends on time or not. 

In particular, the fact that the time independent Hamiltonian itself is a constant of motion ([[How to Solve for Constants of Motion]]) the energy readily follows $\{H,H\} = 0$. For a time dependent Hamiltonian:

$$\begin{gather}\dot E = \dot H = \frac{\partial H}{\partial t} \end{gather}$$