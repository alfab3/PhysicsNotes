To acquire the Green's function for the [[Diffusion Equation]]

Motivated by the observation that diffusion tends to "erase" the "memory" of initial conditions, let us assume that the initial $\phi(x,t=0)$ is localized at some region $|x| < L$ around $x=0$ and consider a time $t >> L^2/D$ and points $|x|>>>L$. We expect then that $\phi(x,t)$ barely depends on the specfic initial profile but only on the ratio $\frac{x}{\sqrt{DT}}$. Namely $\phi(x,t) = F(\xi)$ where $\xi = \frac{x}{\sqrt{DT}}$ is a scaling variable Noting that $$\begin{align} \frac{\partial \phi}{\partial t} = \frac{d \xi}{d t} \frac{dF}{d \xi} = -\frac{1}{2}\frac{x}{\sqrt{DT}}\frac{1}{t}\frac{dF}{d\xi} \\ \text{and} \\ \frac{\partial^2 \phi}{\partial x^2}=\left(\frac{d \xi}{dx}\right)^2\frac{d^2 F}{d\xi^2} = \frac{1}{Dt}\frac{d^2F}{d\xi^2}\end{align}$$

we obtain that the diffusion equation becomes an ODE for $F(\xi)$:

$$\begin{align} \frac{d^2F}{d\xi^2} +\frac{1}{2}\xi \frac{dF}{d\xi} = 0\end{align}$$