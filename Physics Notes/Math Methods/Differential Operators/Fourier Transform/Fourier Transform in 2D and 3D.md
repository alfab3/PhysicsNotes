In 1D [[Fourier Transform]] we saw that for $x \in (-\infty,\infty)$ the set of [[Eigenfunctions]] of the operator $$\begin{align} \mathcal{L} = -\frac{d^2}{dx^2}\end{align}$$ is $u_k(x)\propto e^{ikx}$.

The generalization to higher spatial dimensions is the [[Basis]] given by Eigenfunctions of the operator $$\begin{align} \mathcal{L} = -\nabla^2 \end{align}$$

It is:

$$\begin{align} f(\vec{r}) = \int^\infty_{-\infty}\frac{1}{(2\pi)^n} e^{i\vec{k}\vec{r}} g(\vec{k})d\vec{k}\end{align}$$
and
$$\begin{align} g(\vec k) = \int^\infty_{-\infty} e^{-i\vec k \vec r}f(\vec r)d\vec r\end{align}$$

Such problems deal with axial and rotational symmetries.

### 3D
$$\begin{align} g(k) = \int e^{-i\vec k \vec r} f(r) d\vec r \end{align}$$

Note that $\vec k$ is a parameter in the integral. Hence, let us choose the $\hat 
z$ axis in real space $(\vec r = (x,y,z))\; \text{as} \;\frac{\vec k}{|\vec k|}$

Using spherical coords: $d \vec{r} = d V = r^2 \sin\theta \ dr \ d\theta \ d \phi$ 

Where $0 \leq r < \infty$, $0 \leq \theta \leq \pi$, $0 \leq \phi \leq 2 \pi$
Hence: 
$$\begin{align} g(k) = \frac{4 \pi}{k}\int^\infty_0 dr \ r\ f(r)\sin(kr) \\ f(r) = \frac{1}{2\pi^2}\frac{1}{r}\int^\infty_0 dk \ k \ g(k) sin(kr)\end{align}$$

Conclusion: 
For rotationally-symmetric functions the [[Fourier Transform]] and inverse reduce to integrals over a single variable.

### 2D
Now: $d \vec r = dA =r \ dr \ d\phi$

$$\begin{align} g(k) = 2\pi\int^\infty_0 r d(r) J_0(kr) \\ f(r) = \frac{1}{2\pi}\int^\infty_0 kg(k)J_0(kr)\end{align}$$

Where $J_0(kr)$ is the 1st [[Bessel Functions]] of order 0