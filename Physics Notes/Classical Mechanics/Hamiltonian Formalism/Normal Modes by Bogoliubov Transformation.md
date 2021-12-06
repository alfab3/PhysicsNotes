An equilibrium solution of the equation of motion is the solution that does not evolve in time. By the Hamiltonian equations of motion ([[Hamiltonian Function and Hamilton's Equations]]), the equilibrium solution corresponds to such a point, $\{a_s^{(0)}\}$ in the space of variables $\{a_s\}$ where for any $s$ 
$$\begin{gather} \frac{\partial H}{\partial a_s} = \frac{\partial H}{\partial a_s^*} =0\end{gather}$$

We see that the equilibrium points are the points of extremal behavior of the Hamiltonian.

At the equilibrium point $\{a_s^{(0)}\}$ a natural question arises of what happens if the state of the system is slightly perturbed. The general way of answering this question is to expand the Hamiltonian in the vicinity of the equilibrium in terms of the shifted variables, $a_s \rightarrow a_s - a_s^{(0)}$, assuming that their absolute values are small enough. Omitting the dynamically irrelevant constant term, the resulting Hamiltonian reads
$$\begin{gather} H = \sum_{ij}\left(A_{ij}a^*_ia_j + \frac{1}{2}B_{ij}a_ia_j +\frac{1}{2}B^*_{ij}a^*_ja^*_j\right) \\ A_{ij} = \frac{\partial^2  H}{\partial a_i\partial a_j^*}, \;\; B_{ij} = \frac{\partial^2 H}{\partial a_i\partial a_j}\end{gather}$$

(Linear terms of the expansion are zero). Given (a) that the Hamiltonian has to be real and (b) that we can always symmetrize ([[Symmetric Matrix]]) the matrix $B$ in the case when it is not symmetric automatically, from now on we will assume, without loss of generality that:

$$\begin{gather}A_{ij} = A^*_{ji}, & B_{ij} = B_{ji} \end{gather}$$

For  all equilibrium points that are (local) minima of the function $H$, the Hamiltonian can be diagonalized ([[Diagonalizable Matrix]])  by the Bogoliubov transformation
$$\begin{gather} b_s = \sum_j (u_{sj}a_j + v_s a^*_j) \end{gather}$$

which is a linear [[Canonical Transformations]] with certain coefficients $u$ and $v$. By definition a Hamiltonian is diagonal with respect to [[Complex Canonical Variables]] if it has the form: 

$$\begin{gather}H = \sum_s\omega_sb_sb_s^* \end{gather}$$

equivalent to a set of non-interacting [[Harmonic Oscillator]]s- the [[Normal Modes]]. We will show how to relate the $u$ and $v$ coefficients to the matrices $A$ and $B$, but first we establish their general properties. An elegant way of doing that is to use the fundamental relations
$$\begin{gather} -\{b_s,b_r^*\} = \delta_{sr}, & \{b_s, b_r \}=0\end{gather}$$
implied by the canonicity of the $b$-variables. The above established fact of invariance of the [[Poisson Brackets]] allows us to perform the calculation of the brackets with the $a$-variables, leading to the following two relations:

$$\begin{gather} \sum_j [u_{sj}u^*_{rj} - v_{sj}v^*_{rj}] = \delta_{sr}, & \sum_j [u_{sj}u_{rj} - v_{sj}v_{rj}] = 0 \end{gather}$$

Now we make sure that the conditions are not only necessary, but also sufficient for the transformation to be canonical. To this end we observe that if coefficients $u$ and $v$ satisfy the above equation, then the inverse transformation is given by 

$$\begin{gather} a_j = \sum_s(\tilde u_{js}b_s + \tilde v_{js}b^*_s), & \tilde u_{js} = u^*_{sj}, & \tilde v_{js} = v_{sj} \end{gather}$$

### Derive the Observation 

Now when we know how to express $a's$ in terms of $b's$, we need to make sure that the canonical relations ([[Canonical Transformations]]) are satisfied; and this is easily seen in the form from the above relation. 

The relations for the transformation read:

$$\begin{gather} \sum_j [\tilde u_{js}\tilde u^*_{ks} - \tilde v_{js}\tilde v^*_{ks}] = \delta_{jk}, & \sum_j [\tilde u_{js}\tilde u_{ks} - \tilde v_{js}\tilde v_{ks}] = 0\end{gather}$$

With the relations this can be written as:

$$\begin{gather} \sum_j [u_{sj}^*u_{sk} - v_{sj}v^*_{sk}] = \delta_{jk}, & \sum_j [u_{sj}^*u_{sk} - v_{sj}v_{sk}^*] = 0 \end{gather}$$

The formalism of [[Poisson Brackets]] proves also convenient for obtaining the equations for the $u$ and $v$ coefficients. We start with the simple relation 

$$\begin{gather} i\{H,b_s\} =\omega b_s \end{gather}$$

We then calculate the Poisson Bracket in the l.h.s with the a-variables:

$$\begin{gather} i\{H,b_s\} = \sum_{ij}(A_{ji} a_{i} u_{sj} + B^*_{ij}a^*_iu_{sj} - A{ij}a_i^* v_{sj} - B_{ij}a_i v_{sj}) \end{gather}$$

We then arrive at the system of equations:

$$\begin{gather} \sum_i [A_{ij}u_{si} - B_{ji}v_{si}] = \omega_s u_{sj} & \sum_i[B_{ji}^*u_{si} - A_{ji}v_{si}] = \omega v_{sj}\end{gather}$$

Using the vector notation
$$\begin{gather} \ket{u_s} = (u_{s,1}, u_{s,2}, u_{s,3}, \ldots), & \ket{v_s} = (v_{s,1}, v_{s,2}, v_{s,3}, \ldots)  \end{gather}$$

Taking into account the symmetric relations we can write this as:

$$\begin{gather} \begin{cases} A^*\ket{u_{s}} - B\ket{v_{s}} = \omega_s \ket{u_{s}} \\ B^*\ket{u_{s}} - A\ket{v_{s}} = \omega_s \ket{u_{s}} \end{cases} \end{gather}$$

We can also write this system in terms of $\tilde u's$ and $\tilde v's$, Introducing the vectors:

$$\begin{gather} \ket{\tilde u_s} = (\tilde u_{1,s},\ldots), & \ket{\tilde v_s} = (\tilde v_{1,s},\ldots)\end{gather}$$

we have 
$$\begin{gather} \begin{cases} A\ket{\tilde u_{s}} + B^*\ket{\tilde v^*_{s}} = \omega_s \ket{\tilde u_{s}} \\ B\ket{\tilde u_{s}} + A^*\ket{\tilde v^*_{s}} = -\omega_s \ket{u_{s}} \end{cases} \end{gather}$$

The frequencies of the normal modes, $\omega_s$ arise as the eigenvalues of the problem. The relations defined as: 

$$\begin{gather}\braket{u_r| u_s} - \braket{v_r|v_s} = \delta_{sr} & \braket{v^*_r|u_s} - \braket{u^*_r|v_s} = 0 \\ \braket{\tilde u_r| \tilde u_s} - \braket{\tilde v_r|\tilde v_s} = \delta_{sr} & \braket{\tilde v^*_r|\tilde u_s} - \braket{\tilde u^*_r|\tilde v_s} = 0
\end{gather}$$

are automatically guaranteed at $\omega_r \neq \omega_s$, provided the normalization is fixed by one of the two equivalent conditions:

$$\begin{gather} \braket{u_s|u_s} - \braket{v_s|v_s} = 1 \\ \braket{\tilde u_s|\tilde u_s} - \braket{\tilde v_s|\tilde v_s} = 1\end{gather}$$

This system is invariant with respect to the transformation 
$$\begin{gather} \ket{u_s} \to \ket{v^*_s}, & \ket{v_s} \to \ket{u_s^*}, & \omega_s \to -\omega_s \end{gather}$$

This means that each solution has its counterpart of the opposite frequency.