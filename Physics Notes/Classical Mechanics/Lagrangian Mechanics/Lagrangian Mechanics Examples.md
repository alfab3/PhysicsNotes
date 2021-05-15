One Degree of Freedom
Consider, for example, Atwood's machine. This device, invented in 1784 but still a familiar sight in teaching laboratories is used to demonstrate Newton's laws of motion and to measure $g$. It consists of two weights connected by a light string of length $l$ which passes over a light and frictionless pulley. 

The elementary approach is to write an [[Equations of Motion]] for each of the two weights

$$
m_1\ddot{x_1} = m_1g - T
$$
$$
m_2\ddot{x_2} = m_2g - T
$$

We then take into account the constaint $\dot{x}_1 = -\dot{x}_2$ and eliminate $\ddot{x}_2$ in the favour of $\ddot{x}_1$

$$
m_1\ddot{x_1} = m_1g - T
$$
$$
-m_2\ddot{x_1} = m_2g - T
$$
Finally we eliminate the constaint force, the tension $T$, and obtain the acceleration 
$$
(m_1 + m_2)\ddot{x_1} = (m_1-m_2)g
$$
Lagrange's solution ([[Lagrangian Mechanics]]) takes the constaint into account from the very beginning by introducing a single generalized coordinate $q = x_1 = l - x_2$ and writing 
$$
L = T - V = \frac{1}{2}(m_1+m_2)\dot{q}^2 - (m_2 - m_1)gq
$$

From this we obtain a single equation of motion
$$
\frac{d}{dt}(\frac{\partial L}{\partial \dot{q}^i})-\frac{\partial L}{\partial q^i} = 0 \rightarrow (m_1+m_2)\ddot{q} = (m_1-m2)g
$$
The advantage of the Lagrangian method is that constraint forces, which do no work, never appear. The disadvantage is exactly the same: if we need to find the constaint forces - in this case the tension in the string - we can not use Lagrange alone. 

Lagrange provides a convenient way to derive the equations of motion in non-cartesian coordinate systems such as plane polar coordinates.

Consider the central force problem with $F_r = - \partial_r V(r)$. Newton's method begins by computing the acceleration in polar coordinates. This is most easily done by setting $z=re^{i\theta}$ and differentiating twice: 
$$
\dot{z} = (\dot{r}+ir{\dot{\theta}})e^{i\theta}
$$
$$
\ddot{z} = (\ddot{r}-r{\dot{\theta}}^2)e^{i\theta} + i(2\dot{r}\dot{\theta} + r\ddot{\theta})e^{i\theta}
$$
Reading off the components parallel and perpendicular to $e^{i\theta}$ give the radial and angular acceleration
$$
a_r = \ddot{r} - r\dot{\theta}^2
$$
$$
a_\theta = r\ddot{\theta} + 2\dot{r}\dot{\theta}
$$
Newton's equations therefore become
$$
m(\ddot{r}-r\dot{\theta}^2) = -\frac{\partial V}{\partial r}
$$
$$
m(r\ddot{\theta}+2\dot{r}\dot{\theta}) = 0 \rightarrow \frac{d}{dt}(mr^2\dot{\theta}) = 0
$$
Setting $l=mr^2 \dot{\theta}$, the conserved angular momentum, and elminationg $\dot{\theta}$ gives 
$$
m\ddot{r} - \frac{l^2}{mr^3} = -\frac{\partial V}{\partial r}
$$
Following Lagrange we first compute the kinetic energy in polar coordinates amd set:
$$
L = T - V = \frac{1}{2}m(\dot{r}^2+r^2\dot{\theta}^2) - V(r)
$$
The Euler-Lagrange equations are now
$$
\frac{d}{dt}(\frac{\partial L}{\partial \dot{r}})- \frac{\partial L}{\partial r} = 0 \rightarrow m\ddot{r} - mr\dot{\theta}^2 + \frac{\partial V}{\partial r} = 0
$$
and coincide with Newton's

The first integral is 
$$
E = \dot{r}\frac{\partial L}{\partial \dot{r}} + \dot{\theta}\frac{\partial L}{\partial \dot{\theta}}-L = \frac{1}{2}m(\dot{r}^2+r^2\dot{\theta}^2) + V(r)
$$
which is the total energy. Thus the constancy of the first integral states that 
$$
\frac{dE}{dt} = 0
$$
or that energy is conserved

Many Degrees of Freedom
The extension of the action principle to many degrees of freedom is straightforward. As an example consider the small oscillations about the equilibrium of a system with N degrees of freedom. We paramatrize the system in terms of deviations from the equilbrium position and expand out to quadratic order. We obtain a Lagrangian 
$$
L = \sum^N_{i,j=1}\{\frac{1}{2}M_{ij}\dot{q}^i\dot{q}^j - \frac{1}{2}V_{ij} q^iq^j \}
$$

where $M_{ij}$ and $V_{ij}$ are $NxN$ symmetric matrices encoding the intertial and potential energy properties of the the system. Now we have one equation
