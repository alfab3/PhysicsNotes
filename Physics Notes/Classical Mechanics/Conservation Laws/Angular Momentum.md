The total angular momentum is conserved by any theory satisfying Eqs (2), (4), (5). The idea of the proof is to form the vector product([[Cross Product]]) of $r_i$ with the $i$-th equation in (2), then sum over all $i$'s and finally employ [[The Chain Rule]] to identify [[Time Derivative]]s to show that 
$$
\dot{L}=0
$$
When proving this it is crucial to take into account the force being equal to the derivative of the [[Potential Energy]] as well as some other [[Vectors]] properties. The details of the proof are as follows
$$
\sum^N_{i=1} m_i \vec{r_i} \times \ddot{\vec{r}} = \sum_{i,j} \vec{r_i}\times \vec{F_{i,j}}
$$
First we note that 
$$
\frac{d}{dt}(\vec{r_i}\times\vec{p_i}) = m_i \vec{r_i} \times \ddot{r_i}+ m_i \dot{\vec{r_i}} \times \dot{\vec{r_i}} = m_i\vec{r_i}\times \ddot{\vec{r_i}}
$$
We see that the left hand side is $\dot{\vec{L}}$, and now we need to make sure that 
$$
\sum_{i,j}\vec{r_i} \times\vec{F_{ij}} = 0
$$

If we shift the coordinates of all the particles by a vector $\vec{r_0}$
$$
\vec{r_i}\rightarrow\vec{r_i}+\vec{r_0}
$$
then the angular momentum transforms as 
$$
\vec{L}\rightarrow\vec{L}+\vec{r_0}\times\vec{P}
$$

