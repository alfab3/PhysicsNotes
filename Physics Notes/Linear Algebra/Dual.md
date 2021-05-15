In mathematics, any vector space $V$ has a corresponding dual vector space (or just dual space for short) consisting of all linear forms on $V$, together with the vector space structure of pointwise addition and scalar multiplication by constants.

The dual space as defined above is defined for all vector spaces, and to avoid ambiguity may also be called the algebraic dual space. When defined for a topological vector space, there is a subspace of the dual space, corresponding to continuous linear functionals, called the continuous dual space.

The Dual Space $V^*$ of the vector space ([[Linear Vector Spaces]]) is the set of the linear maps $\bra{w}:V\rightarrow F$ These maps are called "one forms" or covectors. 

Using linearlity, we have, $\forall \ket{v} = v^\mu \ket{e_\mu}$ 

$$\braket{w|v} = \bra{w}(v^\mu)\ket{e_\mu} = v^\mu \braket{w|e_\mu} \equiv v^\mu w_\mu$$

where the n numbers $w_\mu \equiv \braket{w|e_\mu}$ define, once a basis $\ket{e_\mu}^\mu$ is givens uniquely the covector $\bra{w}$.

Given a basis of vectors $\ket{e_1}, ..., \ket{e_n}$ we can define a Dual Basis of covectors $\bra{\theta^1},...,\bra{\theta^n}$, such that 
$$\braket{\theta^\mu | e_\nu} = \delta^\mu_\nu$$ where 

$$\delta^\mu_\nu = 1 \; if \; \mu = \nu
\; 0 \; if \; \; \mu \neq \nu$$

is the kronecker delta. 

It is straightforward to see that $\theta^\mu$ is a basis of $v^*$.

From this, it follows that $dim(V^*) = dim(V)$ and that there is a canonical identificiation between the two spaces: $(V^*)^* \cong V$