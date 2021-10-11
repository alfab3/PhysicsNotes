[[Span]]
[[Linear Independence]]
A subset $S \subseteq V$ where $V$ is a normed vector space ([[Linear Vector Spaces]]) is Dense if 
$$
\forall \; \vec{x} \in V, \epsilon > 0, \exists \; \vec{y} \in S | \; ||\vec{x}-\vec{y}|| < \epsilon
$$
[[Dense Set]]

A subset $S \subseteq V$ is complete if $span(S)$ is dense in $V$. A basis of a Hilbert space is a complete and linearly independent subset

A Basis of a [[Hilbert Space]] is a complete and linearly independent subset.

A set $S$ is countable if there is an injective function
$$
f: S \rightarrow \mathbb{N}
$$
(i.e. if we can label the elements of $S$ with naturals: 1, 2, 3, ...)

A normed vector space is separable if it has a countable and dense subset. Once we have a countable basis we can construct an orthonormal one using [[Gram-Schmidt Orthonormalization]] 

Now let us extend to infinite dimensional basis an important property of finite dimensional ones

Theorem: any vector $\vec{y}$ can be decomposed uniquely on a given basis: given a countable orthonormal basis: $\vec{e_1}, \vec{e_2}, ...,$
$$
\forall \; \vec{y} \in V, \vec{y} = \sum^\infty_{i=1} y_i \vec{e_i}
$$
Proof(for an [[Inner Product Spaces]])
for any fixed $n \in \mathbb{N}$ define 
$$
\Delta_n:= ||\vec{y} - \sum^n_{i=1} y_i \vec{e_i}||^2
$$ 
for some $y_1,...,y_n \in \mathbb{C}$ 
We want to fint the values of $y_i$ that minimize $\Delta_n$

To do so we use $||\cdot||^2=\braket{\cdot,\cdot}$

$$
\Delta_n = \braket{\vec{y},\vec{y}}-\sum^n_{i=1}y_i\braket{\vec{y},\vec{e_i}}-\sum^n_{i=1}y^*_i\braket{\vec{e_i},\vec{y}} + \sum^n_{i,j=1}y^*_iy_j\braket{\vec{e_i},\vec{e_j}}_{\delta_{ij}} = ... 
$$
$$
= \braket{\vec{y},\vec{y}}-\sum^n_{i=1}|\braket{\vec{e_i},\vec{y}}|^2 + \sum^n_{i=1} |y_i-\braket{\vec{e_i},\vec{y}}|^2 \geq \braket{\vec{y},\vec{y}} - \sum^n_{i=1}|\braket{\vec{e_i},\vec{y}}|^2
$$
Where the equality holds for $y_i = \braket{\vec{e_i},\vec{y}}$

This way we have found a formula that allows us to compute the coefficients $y_i$ for any finite $n$ Since the formula does not depend on $n$, we can send $n \rightarrow \infty$

More precisely, since the basis $\{\vec{e_1}, \vec{e_2}, ..., \vec{e_n}, ... \}$ is complete there is a subset $\{\vec{e_{m1}}, \vec{e_{m2}}, ..., \vec{e_{mn}}, ...\}$ $m_1 < m_2< ... < m_n$ such that $\exists \vec{x} \in span(\{\vec{e_{m1}}, \vec{e_{m2}}, ..., \vec{e_{mn}}, ...\})$
with $||\vec{y}-\vec{x}|| < \epsilon$

