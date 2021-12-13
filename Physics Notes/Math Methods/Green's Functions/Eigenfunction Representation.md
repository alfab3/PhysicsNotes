Let us recall the [[Eigenfunctions]] representation of [[Linear Differential Operator]]s. Namely, the [[Completeness Condition]] that the identity operator, namely [[Dirac Delta Function]], can be represented as: 

$$\begin{gather}\delta(x-\xi)  = \sum^\infty_{n=1}\phi_n(x)\overline{\phi_n}(\xi)\end{gather}$$

and it goes that: 

$$\begin{gather} \mathcal L_x \sum^\infty_{n=1}\lambda_n\phi_n(x)\overline\phi_n(\xi) \end{gather}$$

We can ask now is there a similar representation of $\mathcal L^{-1}_x$, namelt $G(x,\xi)$:

$$\begin{gather} G(x,\xi) = \sum^\infty\lambda^{-1}_n \phi_n(x) \overline{\phi}_n(\xi)\end{gather}$$

We readily note the caveat in the above result if $\mathcal L$ is "non-invertible" (has zero-modes).

How to fix: 
Assume $y$ has independent zero modes: 
$$\begin{gather}\phi_1(x),...,\phi_k(x) \end{gather}$$ we can construct the modified Green's function
$$\begin{gather}G(x,\xi) = \sum^\infty_{n=k+1} \lambda_n^{-1}\lambda_n\phi_n(x) \overline{\phi_n(\xi)}\end{gather}$$

If 
$$\begin{gather}\int^b_ad\xi G_{mod}(x,\xi)f(\xi) = y(x) \end{gather}$$