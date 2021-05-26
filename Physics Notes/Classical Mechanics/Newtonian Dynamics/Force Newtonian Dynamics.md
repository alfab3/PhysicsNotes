The main axiom of Newtonian Mechanics (known as Newton's Second Law) ([[Newton's Laws of Motion]]) states that the solution to the problem comes from the following system of $N$ equations of motion.

$$
m_i\ddot{\vec{r}} = \sum^N_{j = 1} \vec{F}_{ij}
$$
$$
j \neq i
$$
$$
(i = 1,2,3,...,N)
$$

where $m_i$ is some positive number characterizing the $i-th$ particle, called its mass; the vector $\vec{F}_{ij}$ is called the force exerted to the $i-th$ particle by the $j-th$ particle. The symbol $\ddot{\vec{r}_i}$ stand for the second derivative of $\vec{r}_i$ with respect to $t$, which is called [[Acceleration]] of the $i-th$ particle. 

The force $\vec{F}_{ij}$ describes the interaction of the $i-th$ particle with the $j-th$ one. If $F_{ij} = 0$ then the interaction is absent. In particular if $\vec{F}_{ij} = 0$ for all $j's$, then the $i-th$ particle does not interat with all the other particles, implying a constant velocity. 

To complete the main axiom, we need to say something about the structure $F_{ij}$'s

First, we postulate that $F_{ij}$ is a function of only to variables, $r_i$ and $r_j$. 

Second, we postulate that the forces are given by the gradients of certain scalar functions called interaction potentials 
$$
F_{ij} = -\frac{\partial}{\partial \vec{r_i}} U_{ij} (\vec{r_i},\vec{r_j})
$$