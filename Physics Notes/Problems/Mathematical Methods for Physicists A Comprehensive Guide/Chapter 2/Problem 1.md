Prove every convergent series is Cauchy

Say we have some series $a_n$ that converges to $L$. This means $\forall \; \epsilon > 0 \; \exists \; N \in \mathbb{R}+$ such that $\forall \; n > N  |a_n - L| < \epsilon$

$\{a_n\}$ is Cauchy if $\forall \; \epsilon > 0 \; \exists N \in \mathbb{R}+$ such that $\forall \; n,m > N  |a_n - a_m| < \epsilon$

Proof
Suppose $\{a_n\}$ converges to $L$. Let $\epsilon > 0$. Since $a_n \rightarrow L \; \exists N \in \mathbb{R}+$ such that $\forall \; n > N  |a_n - L| < \frac{\epsilon}{2}$ Then $\forall \; n,m > N  |a_n - a_m| = |a_n - L + L - a_m| \leq |a_n - L| + |L - a_m| = |a_n - L| + |a_m - L| < \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon$