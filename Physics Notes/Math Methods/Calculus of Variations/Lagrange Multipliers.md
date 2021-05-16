Suppose we want to find an extrenum of the functional on the set of functions subject to the boundary conditions and also the constraint that
$$
Q[f] = C
$$ 
where C is a given constant and 
$$
Q[f] = \int^{x_b}_{x_a} q(f,f_x,x)fx
$$
is a given functional

Consider a new functional
$$
\tilde{F}[f] = F[f]-\lambda Q[f]
$$
where $\lambda$ is a fixed real number. Under the constraint $Q[f] = C$, an extremum of the functional $F$ is simultaneously an extremum of the functional $\tilde{F}$, and vice versa since the two differ by the fixed constant $\lambda C$. Now consider a genuine extremum of the functional $\tilde{F}[f] = F[f]-\lambda Q[f]$. At an arbitrary $\lambda$, this genuine extremum is not supposed to have anything to do with the extremum under the constraint. However normally there exists a special choice $\lambda = \lambda_*$, at which the function $f^(\lambda)$ the genuine extremum of the functional satisfies the condition
$$
Q[f^{(\lambda_*)}] = C
$$
Clearly, the function $f^{(\lambda_*)}$is the solution to the original problem, since the genuine extremum automatically implies the extremum under given (and satisfied) constraint. Once we know the value of $\lambda_*$ the problem is solved. And to find find $\lambda_*$ we simply solve the problem of the genuine extremum of the functional with an arbitrary undefined $\lambda$ and the a posteriori find the proper value $\lambda = \lambda_*$.
