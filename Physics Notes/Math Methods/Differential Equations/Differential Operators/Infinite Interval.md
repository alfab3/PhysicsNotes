For concretness let us consider the operator $\mathcal{L} = -\frac{d^2}{dx^2}$ in $x \in [-L/2,L/2]$ with periodic boundary condition $f(-L/2) = f(L/2)$. [[Eigenfunctions]] are $u_n(x) \propto e^ikx$ with $\lambda_n = k^2_n$ and $k_n = \frac{2\pi n}{L}$

Orthonomality implies that $$\begin{align} u_n(x) = \frac{1}{L}e^{ik_nx} \end{align}$$

Now: $$\begin{align}f(x) = \sum^\infty_{n=-\infty} a_nu_n(x) = \int^\infty_{-\infty}dn \ a_n u_n(x) = \int^\infty_{k=-\infty} dk \frac{dn}{dk} a_ku_k(x) \end{align}$$


$$\begin{align}f(x)=\int^\infty_{-\infty}\frac{dk}{2\pi}g(k)e^{ikx} \end{align}$$

Which is the [[Fourier Transform]]