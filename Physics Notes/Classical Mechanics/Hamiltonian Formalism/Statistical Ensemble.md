Instead of dealing with probability density, we will work with a quantity that is proportional to it and is more transparent. We introduce a statistical ensemble a large number $N_{ens}$ of identical and independent systems distributed in accordance with $W(X,t)$. The $i$-th member of the ensemble is represented by its point $X_i$ in the phase space. The crucial observation is that the quantity $N_{ens}W(X,t)$ gives the number density of the point $\{X_i\}$. Hence to find the evolution of $W$ we just need to describe the evolution of the number density of the points $X_i$, which is intuitively easier since each $X_i$ obeys the Hamiltonian equation of motion ([[Hamiltonian Function and Hamilton's Equations]]).

## A toy model

Consider the following dynamical model with just one degree of freedom: 

$$\begin{gather} H = (1/4)(p^2+q^2)^2\end{gather}$$

The equations of motion are: 
$$\begin{gather} \dot q = (p^2 + q^2)p \\ \dot p -(p^2+q^2)q \end{gather}$$

The quantity $\omega = p^2 + q^2$ is a constant of motion, since, up to a numeric factor it is a square root of energy.

We thus have a linear system of equations:

$$\begin{gather} \dot q = \omega p \\ \dot p = - \omega q \end{gather}$$

which is easily solved:

$$\begin{gather} q(t) = q_0\cos\omega t + p_0 \sin \omega t \\ p(t) = p_0\cos\omega t- q_0\sin\omega t \end{gather}$$

where $q_0\equiv q(0), p_0 \equiv p(0)$ and $\omega = p_0^2 + q_0^2$. We see that our system is a non linear harmonic oscillator. It performs harmonic oscillations but in contrast to a linear harmonic oscillator the frequency of oscillations is a function of energy. 