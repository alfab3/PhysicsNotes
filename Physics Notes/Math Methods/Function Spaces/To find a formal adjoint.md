Just use [[Integration by Parts]] until all [[Derivative]]s move from $u$ to $v$ 

Example: 
$$\begin{align} \mathcal{L} = -i\frac{d}{dx} \; \text{with} \; \omega(x) =1 \\ u^* (\mathcal{L} v) = u^*\left(-i\frac{d}{dx} v\right) \\ =\left(i\frac{d}{dx}u^*\right)v - i \frac{d}{dx}(u^* v) \\ = \left(-i \frac{d}{dx}u\right)^* \cdot v + \frac{d}{dx}(-iu^* v) \end{align}$$

Where: $\left(-i \frac{d}{dx}u\right)^* \cdot v \rightarrow (\mathcal{L}^\dagger u)^*v$ and $\frac{d}{dx}(-iu^* v) \rightarrow \frac{d}{dx} Q[u,v]$

Hence $$\begin{align} \mathcal{L}^\dagger = -i\frac{d}{dx} = \mathcal{L} \; \text{and} \; Q[u,v] = -iu^*v\end{align}$$ 

$$\begin{align} \mathcal{L}=-i\frac{d}{dx} \end{align}$$ is formally self - [[Adjoint]] ([[Hermitian]])

Another Example:

$$\begin{align} \mathcal{L} = p_0(x)\frac{d^2}{dx^2} + p_1(x)\frac{d}{dx}+p_2(x) \; \text{with} \; \omega(x) = 1 \end{align}$$

Similar approach yields: 

$$\begin{align} \mathcal{L}^\dagger = p_0(x)\frac{d^2}{dx^2} + (1p_0'(x) - 1)\frac{d}{dx} + [p_0''(x)-p_1'(x)+p_2(x)]\end{align}$$

Formal self-adjointness with $\omega(x)$ of above operator is only if $p_0'(x) = p_1(x)$ and $p_0''(x) = p_1'(x)$ 

$\mathcal{L}$ is self adjoint with $\omega(x) = 1$ only if $$\begin{align} \mathcal{L} = \frac{d}{dx}(p_0 \frac{d}{dx}+p_2(x))\end{align}$$

This is called [[Sturm-Liouville]] operator. 

It turns out that any second order differential operator is formally [[Hermitian]] with a weight function $$\begin{align} \frac{1}{p_0(x)} e^{\int^x_a\left(\frac{p_1(x')}{p_0(x')}\right)}dx'\end{align}$$