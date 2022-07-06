Consider the [[Schrodinger Equation]] in one dimension

$$\begin{gather} -\frac{\hbar^2}{2m}\frac{\partial^2}{\partial x^2}\Psi(x,t) + V(x)\Psi(x,t) = i\hbar\frac{\partial}{\partial t} \Psi(x,t) \end{gather}$$

If $\Psi(x,t)$ is an [[Eigenstate]] of the [[Hamiltonian (QM)]], the solution becomes 
$$\begin{gather} \Psi(x,t) = e^{-iEt/\hbar} \psi(x)\end{gather}$$
and the time derivative $i\hbar \partial/\partial t$ can be replaced by $E$ in Schrodinger's wave equation. Because the time dependence is then simply a phase factor, all observables become fixed in time for eigenstates. For many applications, we will consider the steady-state case by looking for eigenstates. However, the fact that these are eigenstates does not preclude that the currents are zero. One can set boundary conditions such that current enters and exits the boundary, thus resulting in a steady-state solution, but one where the charge moves. 

To find solutions for problems where the potential is continuous it is sufficient to find solutions of the wave equation that have the correct behavior at $x \to \pm \infty$. If the potential is discontinuous at certain points, boundary conditions must be enforced at every point where a discontinuity is formed. 

If the discontinuity is finite (not a [[Dirac Delta Function]] or an infinite square well), the boundary conditions at the discontinuity are: $\psi(x)$ is continuous and $\partial_x \psi(x)$ is continuous

If $\psi$ were discontinuous, the derivative would be infinite at that point and the current would be infinite at the discontinuity, which would make it impossible to enforce the [[Continuity Equation]]. If the first derivative were discontinuous at some point $y$ the second derivative would be infinite at that point. To understand the second boundary conditions we integrate Schrodinger's equation from $x = y -\epsilon$ to $x = y +\epsilon$, where $\epsilon \to 0$. This yields

$$\begin{gather}-\frac{\hbar^2}{2m}\left(\frac{\partial}{\partial x}\psi(x)\Bigg|_{y+\epsilon}-\frac{\partial}{\partial x}\psi(x)\Bigg|_{y-\epsilon}\right) = \int^{y+\epsilon} _{y-\epsilon}dx(E-V(x))\psi(x)\end{gather}$$

We now consider a discontinuity at $y$ and perform the integral over an infinitesimal range centered about $y$. If the potential is finite the integral on the r.h.s vanishes as $\epsilon \to 0$
$$\begin{gather}-\frac{\hbar^2}{2m}\left(\frac{\partial}{\partial x}\psi(x)\Bigg|_{y+\epsilon}-\frac{\partial}{\partial x}\psi(x)\Bigg|_{y-\epsilon}\right) = 0\end{gather}$$

thus demonstrating the requirement that the derivative of $\psi$ be continuous. However if the potential is a delta function, integrating the right hand side of the above equation over the infinitesimal range can yield a finite value. Thus if 

$$\begin{gather} V(x) = \beta\delta(x-y) \end{gather}$$

the boundary condition becomes $$\begin{gather}-\frac{\hbar^2}{2m}\left(\frac{\partial}{\partial x}\psi(x)\Bigg|_{y+\epsilon}-\frac{\partial}{\partial x}\psi(x)\Bigg|_{y-\epsilon}\right) = -\beta\psi(y)\end{gather}$$