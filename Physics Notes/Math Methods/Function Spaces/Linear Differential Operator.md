Our main purpose is to study properties of linear differential operators. Namely:
$$\begin{align} \mathcal{L}\{f(x)\} = p_0(x)\frac{d}{dx_n} +p_1(x)\frac{d}{dx^{n-1}}+...+p_n(x)\end{align}$$

where $p_i(x)$ are some given functions. 

This leads to the [[Eigenvalues]] problem: $$\begin{align} \mathcal{L}\{ f(x)\} = \lambda f(x)\end{align}$$ and its corresponding [[eigenfunctions]] and how these eigenfunctions provide a [[Basis Set]] for a suitable [[Functional Space]].

Identify the operator $$\begin{align} \frac{d^n}{dx^n} \end{align}$$ with the operator $\delta^{(n)}(x-y)=f^{(n)}(x)$ such that the operator $\mathcal{L}$ can be expressed as  $$\begin{align} \mathcal{L}\{f(x)\} = p_0(x)\int^b_a \delta^{(n)}(x-y)f(y)dy + ... + p_n(x)\int^b_a\delta(x-y)f(y)dy\end{align}$$

Recalling that $\delta(x-y)$ is the identity operator on $\infty$-dim [[Vector Space]], this representaion shows that the a diff operator can be reported as an $\infty$ (square) matrix.

