The most important equilibrium solution of Liouville equation ([[Liouville's Equation and Theorem]]) for the distribution function $W(\{q,p\})$ is the Gibbs distribution describing a system in thermal equilibrium - with itself, if the system is macroscopic, or with a heat bath, if the system is essentially finite. Let us derive this distribution. 

Consider a large number of oscillators and introduce a very weak interaction between them. Specifically we require that for any oscillator the energy of its interaction with the other oscillators be much smaller than typical individual energy of this oscillator. Then let the system equilibrate. To a very good approximation which becomes asymptotically exact in the limit of vanishingly weak interaction our macroscopic system can be viewed as a statistical ensemble of individual oscillators each oscillator obeying its individual distribution, having no correlations with the [[Phase Space]] positions of oscillators. This means that if we take any two oscillators, say 1 and 2, their mutual distribution function $W_{12}$ factorizes, thereby respecting the above mentioned statistical independence of the two systems:

$$\begin{gather} W_{12} (q_1,q_2, p_1,p_2) =w_1(q_1,p_1) w_2(q_2,p_2) \end{gather}$$

In our case the functions $w_1$ and $w_2$ are the same, because all our elementary systems are the same. In a general case, a macroscopic system can consist of subsystems of absolutely different types. 

For purposes that become clear very soon, it is convenient to write this equation in terms of logarithms of distribution functions:

$$\begin{gather}\ln W_{12}(q_1,q_2, p_1,p_2) = \ln w_1(q_1,p_1) +\ln w_2(q_2,p_2)  \end{gather}$$

Clearly, the factorization property applies to any number and any choice of elementary subsystems. And the subsystems should not necessarily be elementary. For any two composite subsystems, $a$ and $b$ we still have 

$$\begin{gather}\ln W_{ab} (\{q^{(a)},q^{(b)},p^{(a)},p^{(b)}\}) = \ln W_a(\{q^{(a)},p^{(a)}\}) + \ln W_b(\{q^{(b)},p^{(b)}\})\end{gather}$$

Furthermore this relation will still hold true if within each of the two subsystems we take into account interactions between constituents. This observation makes especially good sense if the subsystems $a$ and $b$ are well separated spatially , while all interactions between the elementary oscillators are short ranged. This way we can understand how the treatment of our idealized model generalizes to the case of a realistic macroscopic system.

Now it is time to apply [[Liouville's Equation and Theorem]] which tells is that the equilibrium distribution has to be a constant of motion. The combination of this requirement with the property severely restricts our options. For all the subsystems weakly coupled to each other as well as to the rest of the macroscopic system the logarithm of the distribution function has to be an additive constant of motion up to a certain global factor. In many cases the energy is the only additive constant. For all such cases the equilibrium distribution thus reads

$$\begin{gather} W(\{q,p\})\propto e^{-\beta H(\{q,p\})} \end{gather}$$

This is the Gibbs distribution. The global factor $\beta$ is the only free parameter. It controls the value of the total energy. The temperature is then defined as the quantity inverse to $\beta$:
$$\begin{gather} T = 1/ \beta \end{gather}$$

This definition implies that we use energy units for temperature, which is most natural from theoretical point of view. If temperature is measured in Kelvins, then the relations between $\beta$ and $T$ becomes:

$$\begin{gather} k_BT = 1/\beta \end{gather}$$

where the coefficient $k_B$ is called the Boltzmann constant. There is absolutely no physics associated with $k_B$. 