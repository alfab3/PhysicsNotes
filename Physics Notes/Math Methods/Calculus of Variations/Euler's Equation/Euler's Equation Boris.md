A typical problem arising in connection with a [[Functional]] $F[f]$ is the problem of finding a function $f$ that minimizes or maximizes the functional

Suppose the function $f$ is a local max or min of the functional $F$. Then for any small variation of the function $f$, the variation of the functional has to be sign-definite. Let use see what are the implications of this fact. We introduce the symbol $\delta f(x)$ for an infinitesimal variation of the function $f$ and the symbol $\delta F$ for corresponding variation of the functional $F$. That is
$$\begin{align}
\delta F = F[f+\delta F] - F[f]
\end{align}$$
With a simple observation that 
$$\begin{align}
f\rightarrow f + \delta f \Rightarrow f_x \rightarrow f_x + (\delta f)'
\end{align}$$
we have 
$$\begin{align}
\delta F = \int^{x_b}_{x_a} g(f+\delta f, f_x + (\delta f)',x)dx - \int^{x_b}_{x_a} g(f,f_x,x)dx
\end{align}$$
$$\begin{align}
\delta F = \int^{x_b}_{x_a} A(x)\delta f(x)dx
\end{align}$$
where 
$$\begin{align}
A(x)=\frac{\partial g}{\partial f} - \frac{d}{dx} \frac{\partial g}{\partial f_x}
\end{align}$$
$$\begin{align}
A(x) \equiv \frac{\delta F}{\delta f(x)}
\end{align}$$
This allows us to arrive at the equation 
$$\begin{align}
\frac{\partial g}{\partial f} - \frac{d}{dx}\frac{\partial g}{\partial f_x} = 0
\end{align}$$
Functional of many functions
Now if we are looking for minimum/maximum of the functional F, then by definition we have $\delta F \geq 0$ for a minimum or $\delta F \leq 0$ for a maximum And this is only possible if 
$$\begin{align}
A_j(x) \equiv 0
\end{align}$$
The Euler equation then becomes:
$$\begin{align}
\frac{\partial g}{\partial f^{(j)}} - \frac{d}{dx}\frac{\partial g}{\partial f_x^{(j)}} = 0
\end{align}$$



