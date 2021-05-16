A typical problem arising in connection with a functional $F[f]$ is the problem of finding a function $f$ that minimizes or maximizes the functional

Suppose the function $f$ is a local max or min of the functional $F$. Then for any small variation of the function $f$, the variation of the functional has to be sign-definite. Let use see what are the implications of this fact. We introduce the symbol $\delta f(x)$ for an infinitesimal variation of the function $f$ and the symbol $\delta F$ for corresponding variation of the functional $F$. That is
$$
\delta F = F[f+\delta F] - F[f]
$$
With a simple observation that 
$$
f\rightarrow f + \delta f \Rightarrow f_x \rightarrow f_x + (\delta f)'
$$
we have 
$$
\delta F = \int^{x_b}_{x_a} g(f+\delta f, f_x + (\delta f)',x)dx - \int^{x_b}_{x_a} g(f,f_x,x)dx
$$
...
$$
\delta F = \int^{x_b}_{x_a} A(x)\delta f(x)dx
$$
where 
$$
A(x)=\frac{\partial g}{\partial f} - \frac{d}{dx} \frac{\partial g}{\partial f_x}
$$
$$
A(x) \equiv \frac{\delta F}{\delta f(x)}
$$
This allows us to arrive at the equation 
$$
\frac{\partial g}{\partial f} - \frac{d}{dx}\frac{\partial g}{\partial f_x} = 0
$$
Functional of many functions
Now if we are looking for minimum/maximum of the functional F, then by definition we have $\delta F \geq 0$ for a minimum or $\delta F \leq 0$ for a maximum And this is only possible if 
$$
A_j(x) \equiv 0
$$
The Euler equation then becomes:
$$
\frac{\partial g}{\partial f^{(j)}} - \frac{d}{dx}\frac{\partial g}{\partial f_x^{(j)}} = 0
$$
