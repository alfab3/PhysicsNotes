There are an infinite set of [[Eigenfunctions]] and corresponding [[Eigenvalues]]:

$$\begin{align} \mathcal{L}\{u_n(x)\} =\lambda_n u_n(x) \end{align}$$


All [[Eigenvalues]] $\{\lambda_n\}^\infty_{n=1}$ are real.

Eigenfunctions (upon normalization) are orthonormal:

$$\begin{align} \braket{u_n, u_m} = \int_a^b \omega(x)\overline{u}(x)u_m(x) =\delta_{n,m}\end{align}$$

Where $\delta_{n,m}$ is [[Kronecker Delta]]


The [[Orthonormal Basis]] $\{u_n(x)\}^\infty_{n=1}$ is complete. 
For any $y(x) \in L_2[a,b]$ $$\begin{align} ||y(x) - \sum ^N_{n=1} a_nu_n(x)|| \to 0 \end{align}$$

where $a_n = \braket{y,u_n}$

Compatibility Condition: 

Consider orthonormal basis $$\begin{align} \{u_n(x)\}^{\infty}_{n=1} \end{align}$$
of functions in $x \in [a,b]$

Then the basis is complete if $$\begin{align} \sum^\infty_{n=m} u_n(x)\overline{u}_n(y)=\delta(x-y)\end{align}$$