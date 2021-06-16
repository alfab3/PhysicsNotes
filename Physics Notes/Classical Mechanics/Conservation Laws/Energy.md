The quantity 
$$
E = \sum^N_{i=1}\frac{m_i\vec{v_i}^2}{2}+\sum_{i<j}U_{ij}(|\vec{r_i}-\vec{r_j}|)
$$
is called the energy of the system; it is conserved in any theory satisfying Eqs. 2,4,5. To get an idea of the consequences of the energy conservation, consider separately the two terms of equation up top.

Kinetic Energy:
$$
E_{kin} = \sum^N_{i=1}\frac{m_i\vec{v_i}^2}{2}
$$

Potential energy:
$$
E_{pot} = \sum_{i<j}U_{ij}(|\vec{r_i}-\vec{r_j}|)
$$

Given the fact that kinetic energy is non-negative, the conservation of energy imposes serious qualitative constraints on the motion of the system. For example, for a system of two particles attracting each other by a potential $U_{12}(r)<0$ such that $U_{12}(r)\rightarrow 0$ at $r \rightarrow \infty$, the interparticle distance can diverge during the evolution only if $E \geq 0$ Otherwise, there is always an upper bound $r_*$ for the interparticle distance given by $U_{12}(r_*)=E$. 

To prove the energy conservation, multiply the i-th equation in (2) by $\dot{\vec{ri}}$, sum all the equations up, and finally identifying corresponding pieces of the sum with corresponding chain-rule expressions for time derivatives explicitly show that
$$
\frac{dE}{dt} = 0
$$
