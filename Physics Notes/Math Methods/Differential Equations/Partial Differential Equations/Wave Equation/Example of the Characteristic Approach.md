### Statement of the Problem
Consider a bead of mass $M$ that can slide without friction on a rigid rod. The bead is pulled by a long string with tension $T$, and mass density $\rho$

Question: obtain an equation of motion for the bead: $M\ddot y = ???$ where ??? is expressed through $y,\dot y$ and the string constants $T$ and $\rho$

### Solution
The mass is coupled to the string
$$\begin{gather} y(t) = u(x=0,t)\end{gather}$$ and consequently $$\begin{gather} \dot y = \frac{\partial u}{\partial t}\Bigg|_{x=0,t}\end{gather}$$

Now $u(x,t)$ is a solution of the [[Wave Equation]] (with $C = \sqrt{\frac{T}{\rho}}$), hence: $$\begin{gather} u(x,t) = f(x-ct) + g(x+ct) \end{gather}$$

However since the wave only propagate to the right: $g(\zeta) = 0 \Rightarrow u (x,t) = f(x-ct)$

$$\begin{gather}\dot y = \frac{\partial u}{\partial t}\bigg|_{x=0,t} = -cf'(-ct) \Rightarrow f'(-ct)=-\frac{\dot y}{c} \end{gather}$$

Now the vertical force exerted on the mass by the string is $$\begin{gather} F_v \approx -T\frac{\partial u}{\partial x}\bigg|{x=0} \approx-T\cdot f'(-ct)\end{gather}$$

Newton's 2nd equation is:

$$\begin{gather} M\ddot y = F_v \approx -T\cdot f'(-ct)\approx -\frac{T}{C}\cdot \dot y \\ \Rightarrow M\ddot y+\left(\frac{T}{C}\right)\dot y = 0\end{gather}$$

Physically the kinetic energy of the particle is dissipated to radiation implying overdamped dynamics