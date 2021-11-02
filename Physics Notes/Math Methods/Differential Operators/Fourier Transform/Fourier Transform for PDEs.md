[[Definition]]

Consider [[Diffusion Equation]] (in 1D) 

$$\begin{align} \frac{\partial \phi}{\partial t} =D \frac{\partial^2 \phi}{\partial x^2} \end{align}$$

$\phi(x,t)$

under I.C. $\phi(x,t=0) = f(x)$

Write $$\begin{align} f(x) = \frac{1}{2\pi}\int^\infty_{-\infty} dk \tilde\phi(k,t)e^{ikx}\end{align}$$

and consider the spatial Fourier transformation at time $t$:

$$\begin{align} \phi(x,t) = \frac{1}{2\pi}\int^\infty_{-\infty} dk \tilde\phi(k,t)e^{ikx}\end{align}$$

Substituting in the diffusion equation we get:

$$\begin{align} \frac{1}{2\pi}\int^\infty_{-\infty}dk \frac{\partial \phi}{\partial t} (k,t) = D\frac{1}{2\pi}\int^\infty_{-\infty}dk (-ik)^2 \tilde\phi(k,t) \\\frac{\partial \tilde \phi}{\partial t}=-Dk^2\tilde\phi\\ \Rightarrow \tilde \phi = \tilde \phi(k,t=0)e^{-Dk^2t}\end{align}$$

Now to find $\phi(x,t)$ let us use the inverse transform:
$$\begin{align} \phi(x,t) = \frac{1}{2\pi}\int^\infty_{-\infty}dk  \tilde \phi (k,t =0)e^{ikx-Dk^2t}\end{align}$$

Using the definition of the inverse [[Fourier Transform]] to solve for $\tilde \phi$ we arrive at:

$$\begin{align} \phi(x,t) = \int^\infty_{-\infty} d\xi f(\xi) \int^\infty_{-\infty}dke^{ik(x-\xi)-Dk^2t}\end{align}$$

Where the second integral can be solved using the [[Gaussian Integral Trick]]:

$$\begin{align}\int^\infty_{-\infty}dke^{ik(x-\xi)-Dk^2t} = \frac{1}{\sqrt{2\pi Dt}}e^{-\frac{1}{4Dt}(x-\xi)^2} \end{align}$$

Denoting:

$$\begin{align} G(x-\xi,t) \equiv \frac{1}{\sqrt{2\pi Dt}}e^{-\frac{1}{4Dt}(x-\xi)^2}\end{align}$$

We now have: $$\begin{align} \phi(x,t) = \int^\infty_{-\infty} d\xi \phi(\xi,t=0) \ G(x - \xi,t)\end{align}$$

Note that the PDE (involves partial derivatives with respect to $t$ and $x$) for $\phi(x,t)$ becomes an ODE (only time dependent) for $\tilde \phi(k,t)$

Note that the diffusion equation is a conservation equation

Namely it has the form $$\begin{align} \frac{\partial \phi}{\partial t} = - \frac{\partial}{\partial x} J \{\phi\}\end{align}$$

Where $J$ is the [[Flux]].

and $$\begin{align} J = -D\frac{\partial \phi}{\partial x}\end{align}$$

All conservation laws in physics are described by such equations, that is:

$$\begin{align} \frac{\partial}{\partial t} \int^\infty_{-\infty} \phi(x,t) dx = \int^\infty_{-\infty} -\frac{\partial}{\partial x}J \ dx = -J(x,t)\bigg|^\infty_{-\infty}\end{align}$$

Namely the "density" $\phi(x,t)$ at each $x$ may vary in time, but the "total" $\phi$ integrated over space, remains constant

The form of Diffusion equation in higher spatial dimensions $\phi(\vec x, t)$ $$\begin{align} \frac{\partial \phi}{\partial t} = D \nabla^2 \phi \end{align}$$
Where $\nabla^2$ is the Laplacian Operator
