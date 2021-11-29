In Hamiltonian ([[Hamiltonian Function and Hamilton's Equations]]) formalism, dealing with cyclic variables is particularly convenient. Suppose $q_0$ is a cyclic variable: 

$$\begin{gather} \frac{\partial H}{\partial q_0} = 0\end{gather}$$

The constant of motion associated with this cyclic variable is then nothing but corresponding canonical momentum: 

$$\begin{gather} p_0 = \text{const} \end{gather}$$

This means that the variable $q_0$ can be completely ignored when solving for the time evolution of the rest of coordinates and momenta. After the time evolution of those variables is found, the function $q_0(t)$ is established by explicit integration 

$$\begin{gather} q_0(t) = \int dt \frac{\partial H}{\partial q_0}\end{gather}$$

In certain special cases, the partial derivative $\partial H/\partial p_0$ depends only on $p_0$ and this is a constant of motion, implying that $q_0(t)$ is a linear function of time.

### Integrable Systems

The system is called integrable if there exists a set of canonical variables, such that all the [[Generalized Coordinates]] are [[Cyclic Coordinates]] meaning that all generalized momenta are constants of motion. These very special variables, $\{I_j,\theta_j\}$ are called the action angle variables. Here $I$'s stand for the actions(constants of motion) and $\theta$'s are the angles (cyclic variables). Since the Hamiltonian function of an integrable model depends only on $\{I_J\}$, the equations of motion in terms of $\{I_j,\theta_j\}$ become trivial. Each $I_j$ stays constant, while each $\theta_j$ is a linear function of time:

$$\begin{gather} \dot \theta = \omega_j(\{I\}), \;\;\;\; \omega_j(\{I\}) = \frac{\partial H(\{I\})}{\partial I_j}\end{gather}$$

The variables $\{\theta_j\}$ normally have the meaning of phases, with $\{\omega_j(\{I\})\}$ representing corresponding angular frequencies. Each mode behaves as an independent oscillator, with an important reservation that the frequency $\omega_j$ depends on all $I$'s. The triviality of the time evolution of an integrable system in terms of the action-angle variables does not yet mean that all integrable systems are trivial. The point is that the transformation from the systems natural variables to the action angle variables can be quite sophisticated. A very instructive example is the nonlinear Schrodinger equation. This model happens to be integrable in 1D while being non-integrable in higher dimensions.

