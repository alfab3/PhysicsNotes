The most common orthonormal basis we're familiar with is the [[Fourier Basis]].

The crucial thing to realize about polynomial bases is that the monomials are not orthogonal.

That is consider the basis $u_n(x) = x^n$ on $x \in [0,1]$

Then $$\begin{align} \braket{u_n,u_m}=\int^1_0 dx x^{n+m} \omega(w) \end{align}$$ And there is no $\omega(x)$ for which $\braket{u_n, u_m} = \delta_{n,m}$

Assume we try to approximate a function $f(x)$ $0 \leq x \leq 1$ as a polynomial of order $n$. Namely, we want to find $P_n(x) = a_nx^n + ... a_0$ such that $||f(x)-P_n(x)||$ is minimal. Assume we did this optimization and found $a^x_m,... a_0^x$ Now we consider polynomials of order $2n$ namely we want to find $P_n(x) = a_{2n}x^{2n}+...+a_0$ such that $||f(x)-P_{2n}(x)||$ is minimal.

We have to use [[Gram-Schmidt Orthonormalization]]
Start with $P_0(x) = \frac{1}{||1||}$
where $||1|| = \sqrt{\int^1_0\omega (x)dx}$
and define $$\begin{align} P_{n+1}(x) = \frac{xP_n(x)-\sum^n_{i=0}P_i(x)\braket{P_j,xP_n}}{||xP_n(x) - \sum^n_{i=0P_i(x)}\braket{P_i,xP_n}||}\end{align}$$

This assures that the order of $P_{n+1}$ is larger by 1 than order of $P_n$ order of $P_n is n$

Also assures that $$||P_n|| = 1$$

Also assures that $$\braket{P_n,P_m} = \delta_{n,m}$$ by construction. 

Example: [[Legendre Polynomials]]

