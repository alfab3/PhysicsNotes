[[Linear Differential Operator]]s  are not commutative 

$$\begin{align} \mathcal{L}_1\{u\} = \frac{\partial u}{\partial x} + f(x)u(x) \\ \text{and} \; \mathcal{L}_2 = \frac{\partial}{\partial x}+g(x)\end{align}$$

Then: 
$$\begin{align} \mathcal{L}_1 \cdot \mathcal{L}_2 = \frac{\partial^2}{\partial x^2}  +[f(x)+g(x)]\frac{\partial}{\partial x}+g'(x)+f(x)+g(x)\end{align}$$

whereas $$\begin{align} \mathcal{L}_2 \cdot \mathcal{L}_1 = \frac{\partial^2}{\partial x^2} + [f(x) + g(x)]\frac{\partial }{\partial x} + f'(x) +f(x) + g(x)\end{align}$$

The next thing we mus address is the concept of  [[Conjugate transpose]] called "adjoint" operator of linear  differential operators. This is essential to establishing the operator-analogue of the Hermitian matrices and the corresponding [[Orthonormal Basis]] of [[Eigenvectors]]. A simple way to think of $\mathcal{L}^\dagger$ is an operator whose matrix representation is the [[Transpose]] of the matrix representation of $\mathcal{L}$. 

Consider $\mathcal{L}$ [[Linear Differential Operator]] on $[a.b]$ with some weight function $\omega(x)>0$. Then there exists $\mathcal{L}^\dagger$ such that for any $u(x)$, $v(x)$ sufficiently differentiable:

$$\begin{align} \omega[u^x(x)\mathcal{L}v(x) - v(x)(\mathcal{L}^\dagger u(x))^*] = \frac{d}{dx}Q[u,v] \end{align}$$

for some function $Q$. 

$\mathcal{L}^\dagger$ is the "formal [[Adjoint]]" of $\mathcal{L}$ with weight $\omega(x)$

Specifically if $u(x),v(x)$ are both characterized such that $Q[u,v]\bigg|^{x=b}_{x=a}=0$

then:
$$\begin{align} \int^b_a \omega(x) u(x)^* (\mathcal{L}\cdot v)(x)dx = \braket{u,\mathcal{L} v} = \braket{\mathcal{L}^\dagger u,v} =\int(\mathcal{L^\dagger u})(x)^* \cdot \omega(x)v(x)dx\end{align}$$

Can also be written as $u_i M_{ij}v_j = M_{ji}^* u_i v_j$


