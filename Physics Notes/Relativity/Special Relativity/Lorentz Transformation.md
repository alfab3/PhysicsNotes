## Tensor Notation
In [[Contravariant]] form:
$$\begin{gather} x'^\mu = \sum_\nu \Lambda^\mu_{\ \nu} x^\nu & \mu,\nu = 0,1,2,3 \end{gather}$$ Where: $$\begin{gather} \Lambda^\mu_{\ \nu} = \begin{bmatrix} \gamma & -\gamma\beta & 0 & 0\\ -\gamma\beta &\gamma & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1\end{bmatrix} \end{gather}$$
such  that: 

$$\begin{gather} \sum_{\mu = 0}^3x^\mu x_\mu = c^2t^2 - \vec{r}^2 \end{gather}$$
The reverse Lorentz transformation: $$\begin{gather} \Lambda^\mu_{\ \nu} = \begin{bmatrix} \gamma & \gamma\beta & 0 & 0\\ \gamma\beta &\gamma & 0 & 0 \\ 0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1\end{bmatrix} \end{gather}$$

## Properties
Leaves scalar product invariant: 

$$\begin{gather} xy \equiv x_\mu y^\mu = g_{\mu\nu}x^\mu y^\nu =(x,Gy) = (Lx,GLy) = (Lx)_\mu (Ly)^\mu\end{gather}$$
True $\forall$ two vectors 

$\Rightarrow L^\dagger G L = G$ 

in index notation: $$\begin{gather} g_{\mu\nu} = g_{\alpha\beta} L^\alpha_\mu L^\beta_\nu \end{gather}$$
These are numbers and unlike matrices, commute

$$\begin{gather} x'^\nu = L_\mu^\nu x^\mu \to dx'^\nu = L^\nu_\mu dx^\mu \end{gather}$$
from the invariance of $ds^2$:

$$\begin{gather} g_{\mu \nu} dx^\mu dx^\nu = g_{\mu \nu}dx'^\mu dx'^\nu = g_{\alpha \beta} L^\alpha_\mu dx^\mu L^\beta_\nu dx^\nu\end{gather}$$

[[Adjoint]] transformation $\hat L$: 
$$\begin{gather} (Lx)y\equiv x(\hat L y) \Rightarrow \hat L = G^{-1}L^\dagger G, \hat L L = \mathbb{I} \\ \text{det}(L) = \pm 1 \end{gather}$$

Lorentz Transformations are represented by $4 \times 4$ matrices ([[Tensor Formulation]])

Our properties:

$$\begin{gather} L^{0^2}_0 - \sum_{k=1}^3 L^{k^2}_0 = 1 \\ L^{0^2}_k - \sum^3_{m=0}L^{m^2}_k =-1 & k=1,2,3 \\ L^\rho_\mu g_{p\sigma}L^\sigma_\nu =0 &\mu\neq\nu\end{gather}$$

The 4 column vectors are mutually orthogonal, they form a basis obtained from transforming the basis vectors with $L$

## Inhomogeneous Transformations

These are combinations of homogeneous Lorentz -transformations with translations $$\begin{gather}x' = Lx+a \end{gather}$$
One can combine them: 

$$\begin{gather} x'' = L_1x^1+a_1 = L_1(L_2x+a_2)+a_1 =\\ = L_1 L_2 x + (L_1 a_2 +a_1) = L_{tot} x + a_{tot}\end{gather}$$

In index notation:

$$\begin{gather} x'^\mu = x^\mu+a^\mu \end{gather}$$
Where $a^\mu$ is some constant 4-vector

## Homogeneous Transformations
#### Eigenvalues
$$\begin{gather} Lv =\lambda v \\ (L-\mathbb{I})v = 0 \end{gather}$$
For: 

$$\begin{gather} \begin{cases} Lv_1 = \lambda_1 v_1 \\ Lv_2 = \lambda_2 v_2 \\ Lv =\lambda v \end{cases} \Rightarrow \begin{cases} (Lv_1)(Lv_2) \\ (Lv)^2 = v^2 = \lambda^2v^2 \end{cases} \end{gather}$$
If v is not light-like, $\lambda_1 \neq \lambda_2$: $v_1, v_2 = 0$ 

If $\lambda_1$ is an eigenvalue, so is $1/\lambda$ 