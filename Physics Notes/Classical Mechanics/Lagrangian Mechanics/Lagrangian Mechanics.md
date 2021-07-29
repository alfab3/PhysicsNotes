Classical Mechanics can be recast as a variational condition: the [[Principle of least action]]. The idea is to introduce the [[Lagrangian]] function $L= T - V$ where $T$ is the [[Kinetic Energy]] of the system and $V$ the [[Potential Energy]]. Both expressed in terms of [[Generalized Coordinates]] $q_i$ and their [[Time Derivative]]s $\dot{q}_i$. Then, Lagrange showed the multitude of Newton's $\vec{F}=m\vec{a}$ equations, one for each particle in the system can be reduced to
$$\frac{d}{dt}(\frac{\partial L}{\partial \dot{q}_i}) - \frac{\partial L}{\partial q_i}= 0$$

one equation for each generalized coordinate q. Quite remarkably - given that Lagrange's derivation contains no mention of maxima or minima - we recognize that this is precisely the condition that the [[Action]] [[Functional]] 

$$S[q] = \int^{t_{\text{final}}}_{t_{\text{initial}}} L(t,q_i;q'_i)dt$$

be stationary with respect to variations of the trajectory $q_i(t)$ that leave the initial and final points fixed. 