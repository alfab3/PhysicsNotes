In [[Lagrangian Mechanics]] the time evolution of the system with $N$ degrees of freedom is described by the system of $N$ [[Second Order Linear ODEs]] (the [[Euler-Lagrange Equation]]s) for $N$ [[Generalized Coordinates]] $\{q_j\}$. Mathematically speaking, such a problem is equivalent to a system of $2N$ first-order ordinary differential equations. The simplest way to produce such a system is to introduce $N$ new variables trivially associated with time derivatives of the generalized coordinates:
$$\begin{gather} v_j = \dot q_j\end{gather}$$

The substitutions $\dot q_j \to v_j$ and $\ddot q_j \to \dot v_j$ then convert the Euler-Lagrange equations into first-order differential equations with respect to the variables $\{q_j,v_j\}$. As a result, $N$ modified Euler-Lagrange equations and $N$ trivial equation above form the system of $2N$ first-order differential equations for $2N$ variables $\{q_j,v_j\}$.

In such a system of equations, the roles played by the variables $\{v_j\}$ and the roles played by the variables $\{q_j\}$ are quite different. Indeed the structure of that equation have little in common with Euler-Lagrange equations. However, it turns out and the Hamiltonian formalism is all about this remarkable fact - that the variables $\{v_j\}$ can be replaced with some other variables, $\{p_j\}$, in such a way that the resulting equations of motion (the Hamilton's Equations), the roles played the variables $\{p_j\}$ and $\{q_j\}$ are essentially similar.

The set of new variables is produced by a [[Legendre Transform]] of a multivariable function. And the function being Legendre-transformed is the Lagrangian (in which we replace $\dot q_j$ with $v_j$ for clarity). The new variables $\{p_j\}$ are introduced by the following relations: 
$$\begin{gather} p_j =\frac{\partial \mathcal L(\{q,v\})}{\partial v_j} \end{gather}$$

(The symbol $\{q,v\}$ stands for all the $q's$  and all the $v's$.) $N$ algebraic equations implicitly define $N$ functions such that $$\begin{gather} v_j \equiv v_j(\{q,p\})\end{gather}$$
(The symbol $\{q,p\}$ stands for all the $q's$ and all the $p's$) 

The [[Legendre Transform]] has two distinct but closely related aspects: The transformation of variables generated by a certain function - the function $L(\{q,v\})$ in our case  - is naturally accompanied by the transformation of the generating function itself. Corresponding Legendre transform of $\mathcal L (\{q,v\})$ is the function $H(\{q,p\})$, such that: 

$$\begin{gather} H(\{q,p\}) = \sum_jp_jv_j(\{q,p\}) - \mathcal L (\{q,v(\{q,p\})\})\end{gather}$$

The global sign of r.h.s of this equation is a matter of convention. Mathematically it might be natural to use the opposite sign. In Physics, the sign is chosen in such a way that the function $H(\{q,p\})$ is directly related to the energy of the system. The Legendre transformation features two crucial properties. First it preserves the partial derivatives with respect to all the non-transformed variables 
$$\begin{gather}\frac{\partial H(\{q,p\})}{\partial q_j}=-\frac{\partial \mathcal L(\{q,v\})}{\partial q_j} \end{gather}$$
The second property is as follows: 
$$\begin{gather} \frac{\partial H(\{q,p\})}{\partial p_j} = v_j\end{gather}$$

Here the quantity $v_j$ in the r.h.s of the above equation comes in the form of a function $v_j \equiv v_j(\{q,p\})$. It is easy to see that the Legendre transform is symmetric. (Transforming either way is the same mathematical procedure)

Now combining with these two equations with the [[Euler-Lagrange Equation]]s written in the form:

$$\begin{gather} \dot q_j = v_j \\ \frac{d}{dt}\frac{\partial \mathcal L(\{q,v\})}{\partial v_j} = \frac{\partial \mathcal L(\{q,v\})}{\partial q_j}\end{gather}$$

readily leads to Hamilton's equations:

$$\begin{gather} \dot q_j = \frac{\partial H(\{q,p\})}{\partial q_j} \\ \dot p_j = -\frac{\partial H(\{q,p\})}{\partial q_j}\end{gather}$$

Hamilton's equations provide us with an alternative way of describing time evolution of mechanical systems. Here the key role is played by the function $H(\{q,p\})$ called the Hamiltonian function or simply the Hamiltonian. The variables $\{p_j\}$ are called generalized momenta. Apart from being a function of generalized coordinates and momenta, Hamiltonian can also depend on time. 

The Hamiltonian is a constant of motion: $H(\{q(t),p(t)\}) = \text{const}$ provided $H(\{q,p\})$ does not explicitly depend on time. This has to do with the Hamiltonian being equivalent to the system's energy.

In formal (axiomatic) Hamiltonian Mechanics, also known as canonical formalism, the prime role is played by the Hamiltonian function and the pairs of canonical variables - the pairs of generalized coordinates and momenta. For each canonical pair $(q_j,p_j)$, the Hamiltonian function generates a pair of Hamilton's equations. In fact the difference between generalized coordinates and corresponding generalized momenta is merely terminological. Indeed, either of the two transformations, $q_j \to -q_j$ or $p_j \to -p_j$, changes the signs, thus turning coordinates into momenta and momenta into coordinates. 