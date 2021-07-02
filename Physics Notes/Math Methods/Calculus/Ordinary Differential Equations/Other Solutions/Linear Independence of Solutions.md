The criterion for linear dependence of a set of functions of a variable $x$ is the existence of a relation of the form
$$\begin{align} \sum_\lambda k_\lambda \phi_\lambda (x) = 0\end{align}$$
in which not all the coefficients $k_\lambda$ are zero. The interpretation we attach to this equation is that it indicates linear dependence if its satisfied for all relevant values of $x$. Isolated points or partial ranges of satisfaction of the equation fo not suffice to indicate linear dependence. The essential idea being conveyed here is that if there is linear dependence, the function space spanned by the $\phi_\lambda(x)$ can be spanned using less than all of them. On the other hand if the only global solution of the equation is $k_\lambda = 0$ for all $\lambda$, the set of functions $\phi_\lambda (x)$ is said to be linearly independent. 

If the members of a set of functions are mutually orthogonal, then they are automatically linearly independent. To establish this, consider the evaluation of 
$$\begin{align} S = \braket{\sum_\lambda k_\lambda \phi_\lambda| \sum_\mu k_\mu \phi_\mu} \end{align}$$
for a set of orthonormal $\phi_\lambda$  and with arbitrary values of the coefficients $k_\lambda$. Because of the orthonomality, $S$ evaluates to $\sum_k |k_\lambda|^2$ and will be nonzero unless all the $k_\lambda$ vanish.

We now proceed to consider the ramifications of linear dependence for solutions of [[Ordinary Differential Equation]], and for that purpose it is appropriate to assume that the functions $\phi_\lambda(x)$ are differentiable as needed. Then, differentiating the linear depence criterion equation repeatedly, with assumption that it is valid for all x, we generate a set of equations
$$\begin{align} \sum_\lambda k_\lambda \phi'_\lambda (x) = 0 \\ \sum_\lambda k_\lambda \phi''_\lambda (x) = 0 \end{align}$$
continuing until we have generated as many equations as the number of $\lambda$ values. This gives us a set of homogeneous linear equations in which $k_\lambda$ are the unknown quantities. There is a solution of than all $k_\lambda = 0$ only if the determinant of the coefficients of the $k_\lambda$ vanishes. This means that the linear deoendence we have assumed by the accepting the criterion implies that
$$\begin{align}
	\begin{bmatrix}
		\phi_1 & \phi_2 & \ldots & \phi_n\\
		\phi_1' & \phi_2' & \ldots & \phi_n'\\
		\ldots & \ldots & \ldots & \ldots\\
		\phi_1^{(n-1)} & \phi_2^{(n-1)} & \ldots & \phi_n^{(n-1)}
	\end{bmatrix}
\end{align}$$
This determinant is called the Wronskian, and the analysis leading to the matrix shows that:
1) If the Wronskian is not equal to zero then the criterion has no solution other than $k_\lambda = 0$ The set of functions $\phi_\lambda$ is therefore linearly independent
2) If the Wronskian vanishes at isolated values of the argument, this does not prove linear dependence. However, if the Wronskian is zero over the entire range of the variable, the functions $\phi_\lambda$ are linearly dependent over this range

[[Example 7.6.1 Linear Independence]]
[[Example 7.6.2 Linear Dependence]]