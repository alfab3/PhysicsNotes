To start we note that the taking of a derivative is a linear operation meaning that 
$$
\frac{d}{dx}(a\phi(x)+b\psi(x))=a\frac{d\phi}{dx}+b\frac{d\psi}{dx}
$$
and the derivative operation can be viewed as defining a linear operator: $\mathcal{L}=d/dx$ Higher derivatives are also linear operators. 

Linear differential operators include those of the form
$$
\mathcal{L}\equiv\sum^n_{v=0}p_v(x)\Bigl(\frac{d^v}{dx^v}\Big)
$$
where the functions $p_v(x)$ are arbitrary

An ODE is termed homogeneous if the dependent variable occurs to the same power in all its terms. and inhomogeneous if otherwise; it is termed linear if it can be written in the form 
$$
\mathcal{L}\phi(x)=F(x)
$$
where $\mathcal{L}$ is a linear differential operator and $F(x)$ is an algebraic function of $x$. An important class of ODEs are those that are both linear and homogeneous, and thereby of the form $\mathcal{L}_\phi = 0$.

The solutions to ODEs are in general are not unique and if there are multiplie solutions it is useful to identify those that are linearly independent [[Linear Independence]]. Homogeneous linear ODEs have the general property that any multiple of a solution is also a solution, and that if there are multiple linearly independent solutions, any linear combination of those solutions will also solve the ODE. This statement is equivalent to noting that if $\mathcal{L}$ is linear, then for all $a$ and $b$.
$$
\mathcal{L}_\phi=0 \; and \; \mathcal{L}_\psi = 0 \rightarrow \mathcal{L}(a\phi+b\psi)=0
$$

Further terms used to classify ODEs include their order - highest derivative therein, and degree - power to which the highest derivative appears after the ODE is rationalized.
