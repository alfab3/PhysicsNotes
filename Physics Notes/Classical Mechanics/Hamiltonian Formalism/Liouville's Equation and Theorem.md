## Continuity Equation
Having played with a toy model we are in a good position to address the general case. From now on we normalize the function $W(X,t)$ to the total number of the ensemble members, meaning that the number of points in the phase space volume $\Gamma_0$ at the time $t$ is given by the integral 
$$\begin{gather} N_{\Gamma_0}(t) = \int_{\Gamma_0}W(X,t)d\Gamma \end{gather}$$

Here $d\Gamma = dq_1 ... dq_m dp_1...dp_m$ is the element of the [[Phase Space]] volume; the integration is over the volume $\Gamma_0$ is given by the following time derivative: 

$$\begin{gather} \dot N_{\Gamma_0} = \int_{\Gamma_0}\frac{\partial }{\partial t}W(X,t)d\Gamma \end{gather}$$
By the definition of the function $W(X,t)$, its variable $X$ does not depend on time, so that the time [[Derivative]] deals only with the variable $t$.

An alternative way of calculating $\dot N_{\Gamma_0}$ is by counting the number of points that cross the surface $\Gamma_0$ per unit time:

$$\begin{gather} \dot N_{\Gamma_0} = -\int_{\text{surface of } \Gamma_0} \vec J \cdot d\vec S\end{gather}$$

Here the vector $J$ -directed along the vector $V$ and proportional to it - is the flux of the points $d \vec S = \vec n dS$ where $dS$ is the area of an infinitesimal surface element and $\vec n$ is the outward directed normal vector at this element. 

In accordance with one of the most famous theorems of vector calculus, the surface integral can be converted into the bulk integral: 
$$\begin{gather} \int_{\text{surface of } \Gamma_0} \vec J \cdot d \vec S  = \int_{\Gamma_0} \nabla \cdot \vec J d \Gamma\end{gather}$$

where $\nabla$ is the vector differential operator 
$$\begin{gather} \nabla = \left(\frac{\partial}{\partial x_1},\frac{\partial}{\partial x_2},\frac{\partial}{\partial x_3},...\right) \end{gather}$$

We arrive at the equality $$\begin{gather} \int_{\Gamma_0}\frac{\partial}{\partial t}W(X,t)d\Gamma = -\int_{\Gamma_0}\nabla\cdot \vec J d \Gamma \end{gather}$$

The next step is very standard in vector calculus. Taking into account that the equation about is true for any $\Gamma_0$, including infinitesimally small one, we conclude that $$\begin{gather} \frac{\partial W(X,t)}{\partial t} = - \nabla\cdot \vec J \end{gather}$$

We have arrived at a very general relation, known as the continuity equation. It arises in theories describing flows of the densities of additive conserved quantities.

Since all our particles move with one and the same local velocity $\dot X = V(X)$ from the definition of the particle flux it immediately follows that $\vec J$ is equal to the particle concentration times the local velocity $V(X)$:

$$\begin{gather} \vec J = W(X,t)\dot X = W(X,t) V(X)\end{gather}$$

Substituting this expression for $\vec J$ we get a closed continuity equation for $W(X,t)$: 

$$\begin{gather} \frac{\partial}{\partial t} W(X,t) = - \nabla \cdot [W(X,t)V(X)] \end{gather}$$

Being a first-order differential equation with respect to time the above equation unambiguously describes the evolution of any initial distribution $W(X,t = 0)$. 

### Liouville's Equation
The continuity equation of the above form works for a statistical description [[Phase Space]]. Our final step is to take into account that we are dealing with a rather special phase space - the phase space of [[Hamiltonian Function and Hamilton's Equations]]. Taking into account phase space $X$ and $V$ representations brings us to an elegant result known as Liouville's equation:

$$\begin{gather} \frac{\partial}{\partial t} W(X,t) = \{W,H\}\end{gather}$$

### Liouville's Theorem 
The form of Liouville's equation is reminiscent of:

$$\begin{gather} \dot A = \{H,A\} \end{gather}$$

Nevertheless, the physical meanings of the two relations are quite different. In the L.H.S. of the above equation we have the total time derivative with respect to time, $\dot A \equiv (d/dt)A(\{q(t),p(t)\})$, while the variable $X$ in Louiville's equation is time-independent: $X$ simply a label of a point in the [[Phase Space]]. Note also the different sign: $\{W,H\} = - \{H,W\}$

The combination of the two equations allows us to understand the structure of equilibrium solutions of Louiville's equation. For any equilibrium (=time-independent) solution $W(X)$ we have $\{H,W\} = 0$. Thus if we formally plug $X = X(t)$ into $W(X)$, where $X(t)$ is any trajectory of satisfying the equations of motions then the result will be time-independent. That is, any equilibrium $W$ is formally equal to some constant of motion, and vice - versa.