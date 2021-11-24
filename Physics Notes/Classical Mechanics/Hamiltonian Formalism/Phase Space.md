Suppose we have a dynamical problem of the following mathematical structure:
$$\begin{gather} \dot X = V(X) \end{gather}$$

Here $X = (x_1,x_2,x_3,...)$ is a vector of certain variables that evolve in time. At this point, the nature of the variables, as well as the nature of the system they describe, is not important. What matters is the structure of the equation telling us that if we know $X$ at a certain time moment the further evolution $X$ is unambiguously defined , since we are dealing with a first order differential equation with respect to time. The space of points ([[Vectors]]) $X$ is referred to as phase space. Each point in the phase space belongs tp a unique trajectory. That is two different trajectories cannot share one and the same point of the phase space. The only exception that actually confirms the rule is the point of unstable equilibrium. At such a point, more than one trajectories can  meet. However, none of the trajectories can reach the equilibrium point at any finite time, so it makes perfect sense to speak of open trajectories approaching the point of unstable equilibrium at $t \to \pm \infty$.

For a Hamiltonian ([[Hamiltonian Function and Hamilton's Equations]]) system with $m$ degrees of freedom described by $m$ [[Generalized Coordinates]] and corresponding $m$ generalized momenta, there is a natural $2m$ dimensional phase space formed by the vectors 
$$\begin{gather}X = (q_1,q_2,...,q_m,p_1,p_2,...,p_m) \end{gather}$$

The Hamilton's equations then are naturally written in the form of the phase space structure. 

The Hamilton's equations then are naturally written in the form of the phase structure with:

$$\begin{gather} V = \left(\frac{\partial H}{\partial p_1},...,\frac{\partial H}{\partial p_m}, -\frac{\partial H}{\partial q_1},...,-\frac{\partial H}{\partial q_m}\right) \end{gather}$$

The notion of the phase space is convenient for statistical description of mechanical system. Suppose that the initial state for a system is known only with a certain finite accuracy. The means that actually we know only the probability density $W_0(X)$ of having the point $X$ somewhere in the phase space. If the initial condition is specified in terms of probability density, then the subsequent evolution should be also described probabilistically. That is we have to work with the distribution $W(X,t)$, which should be somehow related to the initial condition $W(X,0) = W_0(X)$.
