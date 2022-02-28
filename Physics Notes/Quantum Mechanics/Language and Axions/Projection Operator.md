# Definition
$\ket{\phi_n}\bra{\phi_n}$ is a projection operator. In some familiar notation say we have: 
$$\vec{v} = v_1\hat{i} + v_2\hat{j} + v_3\hat{k}$$ 

In general terms:
$$\ket{\psi} = v_1\ket{\phi_1} + v_2\ket{\phi_2} + v_3\ket{\phi_3}$$

We have: $\braket{\phi_1 | \psi} = v_1$, but if you want to produce the whole thing with the $\ket{\phi_1}$
$$\ket{\phi_1}\braket{\phi_1|\psi} = \ket{\phi_1}v_1 = v_1\ket{\phi_1}$$
 Where $\ket{\phi_1} \bra{\phi_1}$ is the projection operator. Originally they would use: $\hat{i} \hat{i} \cdot \vec{v} = v_1\hat{i}$ which used to be called the dyadic. 
 Properties:
 $$p_n = \ket{\phi_n} \bra{\phi_n}$$
 $$p_n^2 = \ket{\phi_n} \braket{\phi_n | \phi_n} \bra{\phi_n} = \ket{\phi_n} \bra{\phi_n} = p_n$$
 
 If you have an orthonormal basis formed from these vectors? 
 $$\sum_n \ket{\phi_n} \bra{\phi_n} = \mathbb{I}$$ 
 Which is the unit operator, the unit operator, when acting on a  vector, does nothing at all. 
 
 $$p_n(p_n - \mathbb{I}) = 0$$
 
 [[Eigenvalues]] of projection operators are either 0 or 1. 
 
 At this point we need to explain/remind what we mean by projector ([[Projection Operator]]) $\hat P_\lambda$. If the eigenvalue $\lambda$ is not degenerate then $\hat P_\lambda = \ket{e_\lambda}\bra{e_\lambda}$ where $\ket{e_\lambda}$ is corresponding unit eigenvector of the operator $A$: $A\ket{e_\lambda} = \lambda\ket{e_\lambda}$,$\braket{e_\lambda|e_\lambda} = 1$. In a general case: 

$$\begin{gather} \hat P = \sum_\nu \ket{e_{\lambda,\nu}}\bra{e_{\lambda,\nu}}{}\end{gather}$$

where $\{e_{\lambda,\nu}\}$ is any -does not matter which particular one - ONB in the $\lambda$ - eigenspace of the operator $A$. 

 
 # Properties
 
 The following three properties of the projectors - associated with a certain [[Hermitian]] operator $A$ - are especially important: 

$$\begin{gather} A = \sum_\lambda \lambda \hat P_\lambda \\ \hat P_\lambda \hat P_{\lambda'} = \delta_{\lambda,\lambda'} \hat P_\lambda \\ \sum_\lambda \hat P_\lambda = \hat 1 & \text{completeness relation}\end{gather}$$


where $\hat 1$ is the identity operator. The sum $\sum_\lambda(...)$ is over all $\lambda's$
 