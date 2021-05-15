The fundamental notions of Mechanics are the notions of state (of a closed system), time, and evolution/motion. The closed system does not interact with the rest of the world. 

Speaking generally, by the state one means some mathematical object, $S$ being a function of a real variable $t$, which is called time. The evolution/motion is understood as a change of $S$ with $t$. Finding some function $S(t)$ for a given system is the ultimate goal of mechanics. It is acheived by knowing the state of the system $S(t_0)$ at some initial time moment $t_0$ and utilizing the laws of motion. 

In the Newtonian picture of the world, any system can be viewed as consisting of point objects, particles. Each particle $i$ is characterized by a radius-vector (position) $\vec{r}_i$ in a d-dimensional space. Typically, $d = 3$, since this corresponds to our real world, but this will often be reduced to 2 or 1. If a system consists of $N$ particles then its state is exhaustively descrived by a set of 2N vectors, $S(t) \equiv \{\vec{r_i}(t), \vec{v_i}(t)\}, \; i =1,2,3,...,N$ where $\vec{v_i}$ stands for the [[Derivative]] of $\vec{r_i}$ with respect to time: $$ \vec{v}_i(t) = \frac{d}{dt}\vec{r_i}(t) \equiv \dot{\vec{r_i}}(t)$$

The quantity $\vec{v_i}(t)$ is called the  [[Velocity]] of the $i-th$ particle at the time $t$. The fundamental problem of mechanics is then formulated as follows. Given the positions (radius-vectors) and velocities of all the particles at some moment $t_0$, find the positions and velocities of the particles at any $t>t_0$. The main axiom of Newtonian Mechanics (known as Newton's Second Law) ([[Newton's Laws of Motion]]) states that the solution to the problem comes from the following system of $N$ equations of motion.

$$m_i\ddot{\vec{r}} = \sum^N_{j = 1} \vec{F}_{ij}$$
$$j \neq i$$
$$(i = 1,2,3,...,N)$$

where $m_i$ is some positive number characterizing the $i-th$ particle, called its mass; the vector $\vec{F}_{ij}$ is called the force exerted to the $i-th$ particle by the $j-th$ particle. The symbol $\ddot{\vec{r}_i}$ stand for the second derivative of $\vec{r}_i$ with respect to $t$, which is called acceleration of the $i-th$ particle. 
$$a_i(t) \equiv \ddot{\vec{r}_i}(t) \equiv \frac{d^2}{dt^2}\vec{r}_i = \dot{\vec{v}_i}(t)$$ 
The force $\vec{F}_{ij}$ describes the interaction of the $i-th$ particle with the $j-th$ one. If $F_{ij} = 0$ then the interaction is absent. In particular if $\vec{F}_{ij} = 0$ for all $j's$, then the $i-th$ particle does not interat with all the other particles, implying a constant velocity. 
