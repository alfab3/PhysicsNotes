Consider $\vec{v}$ in [[vector space]] of dimension $n$, and an [[orthonormal basis]] $\{ \vec{v}_j\}^n_{j=1}$ such that $\vec{v} = \sum^n_{j=1} a_j\vec{v}_j$. Consider a [[Subset]] $\{\vec{v_j}\}^k_{j=1}$ with $k < n$. Then the best approximation for $\vec{v}$ with $\{\vec{v}_j\}^k_{j=1}$ is $\vec{v} = \sum^k_{j=1}a_j\vec{v}_j$

Namely define: 
$$\begin{align} err[b_1 - b_k] \equiv ||\vec{v} - \sum^k_{j=1} b_j \vec{v}_j|| \\ min \ err[b_1 - b_k] = ||\sum^k_{k+1=j} a_j \vec{v}_j|| \end{align}$$ and is realized for $\{b_j = a_j\}_{j=1}^k$

