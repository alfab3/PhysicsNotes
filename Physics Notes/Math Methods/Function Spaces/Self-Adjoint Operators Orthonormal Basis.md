Example: $$\begin{align} \mathcal{L} = - \frac{d^2}{dx^2} \; \text{with} \; \omega(x) = 1 \\ \text{s.t.}  \; D(\mathcal{L}) = \{y(x), \; \text{s.t} \; \mathcal{L} y(x) \in L_2[0,1]\} \end{align}$$

Where $D$ is the domain and $y(0) = y(1) = 0$

We can readily check that $$\begin{align} \braket{y_1,\mathcal{L}y_2} =  \braket{\mathcal{L}y_1,y_2} = y_1'^*y_2 - y_1^*y_2'\Bigg|^1_0 = 0\end{align}$$ so that $\mathcal{L}$ is [[Hermitian]]

[[Eigenvalues]] equation: $\mathcal{L} y_n = \lambda_n y_n$ 

$\lambda_n = n^2\pi^2, \; y_n(x) = sin(n\pi x), \; n =1,2,3,...$

Properties
1) All eigenvalues are real
2) $\{y_n(x)\}$ form orthonormal basis (upon [[Normalization]]): $$\begin{align} 2 \int^1_0 \sin(n\pi x) \sin(m \pi x)dx = \delta_{nm}\end{align}$$ (where $\delta_{nm}$ is the [[Kronecker Delta]])
3) For any $y(x) \in L_2[0,1]$: $$\begin{align} y(x) = \sum^\infty_{n=1} a_n \sqrt{2} \sin(n\pi x)\end{align}$$ with $$\begin{align} a_n = \int^1_0 y(x)\sqrt{2}sin(n\pi x)dx \end{align}$$

These are the basic elements of all truly [[Hermitian]] differential operators known as [[Sturm-Liouville]] theory. 

Counter example 

Let us consider again $\mathcal{L} = -i\frac{d}{dx}$ we know already that $\mathcal{L}$ is formally [[Hermitian]]

$\mathcal{L} = \mathcal{L}^\dagger$

Now consider again the domain $$\begin{align} D(\mathcal{L}) = \{y: \mathcal{L}y\in L_2[1,0],y(1) = y(0) = 0\} \end{align}$$

once again we find $$\begin{align} \braket{y_1, \mathcal{L}y_2} - \braket{\mathcal{L}y_1,y_2} = -i(y^*_1 y^2)\Bigg|^1_0 = 0\end{align}$$

Let's to try to find [[Eigenvalues]] vamely consider the equation:
$$\begin{align} \mathcal{L} u_n(x) = \lambda_n u(x) \\ -i\frac{d}{dx} u_n(x) = \lambda_n u(x)\end{align}$$

Solutions are of the form $$\begin{align} u_n(x) = e^{i\lambda_n x} \end{align}$$

which does not satisfy the boundary conditions.

What went wrong?

Since $D(\mathcal{L})$ is limited to functions $y_2(1) = y_2(0)= 0$ the boundary term $Q[y_1,y_2]\bigg|^1_0 = -i \bar{y}_1y_2\Bigg|^1_0 = 0$ regardless of the boundary values specified in the domain of $\mathcal{L}^\dagger$ 

That is: 
$$\begin{align} D(\mathcal{L}^\dagger) = \{y: \mathcal{L} y \in L_2[0,1], (\text{with any BC})\}\end{align}$$

$$\begin{align} D(\mathcal{L}) \neq D(\mathcal{L}^\dagger) \end{align}$$

even though $\mathcal{L} = \mathcal{L}^\dagger$ "formally"