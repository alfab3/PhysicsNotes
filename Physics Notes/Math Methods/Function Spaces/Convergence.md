We are usually forced to use numerical methods, or to expand as a power series in some small parameter for a real world problem. The result is a sequence of approximate solutions $f_n(x)$, which we hope will converge to the desired exact solution $f(x)$

Convergence means that the distance between $f_n$ and the limit function $f$ gets smaller and smaller as $n$ increases.

1) If, for each x in its domain of definition $\mathcal{D}$, the set of numbers $f_n(x)$ converges to $f(x)$, then we say the sequence converges pointwise
2) If the maximum separation 
$$
\sup_{x\in\mathcal{D}}|f_n(x)-f(x)|
$$
goes to zero as $n \rightarrow \infty$, then we say that $f_n$ converges to $f$ uniformly on $\mathcal{D}$
3) If
$$
\int_\mathcal{D} |f_n(x)-f(x)|dx
$$
goes to zero as $n\rightarrow \infty$, then we say that $f_n$ converges in the mean to $f$ on $\mathcal{D}$

Uniform convergence implies pointwise convergence, but not vice versa. If $\mathcal{D}$ is a finite interval, then uniform convergence implies convergence in the mean, but convergence in the mean implies neither uniform nor pointwise convergence.

A sequence 
$$
x_1, x_2,...,x_n,... \in F
$$
converges to $x \in F$ if 
$$
\forall \; \epsilon > 0, \exists N \in \mathbb{N} \;|\; |x_n - x| \leq \epsilon \; \forall \; n \geq N
$$
A sequence of vectors converges $\vec{x_1}, \vec{x_2},..., \vec{x_n}$
converges to $\vec{x} \in V$
with respect to the norm $||\cdot||$ if 
$$
\forall \; \epsilon > 0, \exists N \in \mathbb{N} \;|\; |\vec{x_n} - \vec{x}| \leq \epsilon \; \forall \; n > N
$$

The concept of convergence requires that we know $\vec{x}$ the limit.


