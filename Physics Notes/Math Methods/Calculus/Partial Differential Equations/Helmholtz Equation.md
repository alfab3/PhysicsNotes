An example for using [[Fourier Transform]] for solving PDE is the Helmholtz equation $$\begin{align} -\gamma\nabla^2 h +(\rho g)h=0\end{align}$$

or: $$\begin{align} -\nabla^2h +l_c^{-2}h =0\end{align}$$

where $l_c = \sqrt{\gamma/\rho g}$ 

Here, $\gamma$ is the "surface tension" (or "surface energy")

$\rho$ is the mass density and $g$ is the gravitational acceleration 

Physical Motivation: 
Consider a liquid surface, whose equilibrium shape is $h(x,y) = 0$. Assume the surface is determined, i.e. $h(x,y) \neq 0$. The energy (per unit area) is the additional surface area multiplied by $\gamma$: $\gamma (\sqrt{1+|\nabla h|^2}-1)$ and gravity: $1/2(\rho g)h^2$

Assuming small slope (or long wavelength) namely $|\nabla h|<<1$, we can Taylor expand the square-root $\sqrt{1+|\nabla h|^2} \approx 1 + 1/2|\nabla h|^2$ and obtain the energy functional:

$$\begin{align} U\{h(x,y)\} = \frac{1}{2} \int\int \ dx \ dy (\gamma|\nabla h|^2 + \rho g h^2)\end{align}$$

Minimization of this integral yields the Helmholtz equation as the corresponding [[Euler-Lagrange Equation]]

Assume we deform the liquid surface by placing a thin, but non-straight wire at $y=0$

That is, the BC's for the Helmholtz equation at $y = 0$ is $h(x,y = 0) = f(x)$ Since any $h(x,y) \neq 0$costs energy, we expect that at $|y| \rightarrow 0$ we have $h(x,y) \rightarrow 0$

Hence we need to solve: $$\begin{align} -\left( \frac{\partial^2}{\partial x^2} + \frac{\partial ^2}{\partial y^2}\right) + l_c^{-2}h = 0 \end{align}$$

Where $h(x,y= 0)$ and $h(x,y) \rightarrow 0$ Following similar steps to the Fourier analysis of the diffusion equation we write: 
$$\begin{align} h(x,y) = \frac{1}{2\pi} \int^\infty_{-\infty}dk e^{ikx} \tilde h(k,y)\end{align}$$ substituting in Helmholtz equation we get: 
$$\begin{align} \frac{1}{2\pi} \int^\infty_{-\infty} dk \left[ - (-ik)^2 \tilde h (k,y) - \frac{\partial^2 \tilde h}{\partial y^2}(k,y) + l_c^{-2} \tilde h(k,y) \right]\end{align}$$

and again, orthonormality of [[Fourier Basis]] implies $$\begin{align}\frac{\partial^2 \tilde h}{\partial y^2} - (k^2+l_c^{-2})\tilde h = 0 \end{align}$$. 
That is, the PDE was converted to an ODE for each $k$

Solution: 
$$\begin{align} \tilde h (k,y) = \tilde h (k,0) e^{-\sqrt{k^2+l^{-2}_c}|y|} \\ \tilde h (,0) = \tilde f(k)\end{align}$$

with inverse [[Fourier Transform]] and suitable change of integrals order we obtain th eGreen's function for Helmholtz problem:

$$\begin{align} h(x,y) = \int^\infty_{-\infty} d\xi f(\xi) G(x - \xi,y) \end{align}$$

