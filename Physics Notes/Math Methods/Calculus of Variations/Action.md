A numerical description of how a physical system has changed over time. It is significant because the equations of motion of the system can be derived through the principle of stationary action ([[Principle of least action]]). In the simple case of a single particle moving with a  specified velocity, the action is the momentum of the particle times the distance it moves added up along its path, or equivalently twice the [[Classical Mechanics/Newtonian Dynamics/Kinetic Energy]] times the length of time for which it has that amount of energy added up over the period of time under consideration. 

Mathematical definition 
Using calculus of variations, the evolution of a physical system corresponds to a stationary point of the action.
The action is typically represented as an integral over time, taken along rhe path of the system between the initial time and the final time of the development of the system. 
$$
S = \int^{t_2}_{t_1} L dt
$$
where the integrand $L$ is called the [[Lagrangian]]

In classical physics the term action has a number of meanings. 
Action [[Functional]]
Most commonly the term used for a functional $S$ which takes a function of time and (for fields) space as input and return a scalar. In classical mechanics, the input function is the evolution $q(t)$ of the system between two times $t_1$ and $t_2$, where $\vec{q}$ represents the generalized coordinates. The action $S[q(t)]$ is defined as the integral of the [[Lagrangian]] $L$ for an input evolution between the two times:
$$
S[q(t)] = \int^{t_2}_{t_1} L(\vec{q}(t),\dot{\vec{q}}(t),t)dt
$$
where the endpoints of the evolution are fixed and defined as $\vec{q}_1 = \vec{q}(t_1)$ and $\vec{q}_2 = (\vec{q})t_2$