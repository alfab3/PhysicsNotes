A different notion of convergence, that does not require the knowledge of $\vec{x}$ is the following

A sequence of real numbers: $\{a_n\}^\infty_{n=1}$ is called a Cauchy Sequence if for every $\epsilon > 0$ there is a natural number $N \in \mathbb{N}$ such that if $m,n \geq N$ then
$$
|a_m - a_n| < \epsilon
$$

Ex: 
$$
a_n = \frac{n}{n+1}
$$
is Cauchy

Work:
We want 
$$
|a_n - a_m| < \epsilon
$$

Where $\epsilon$ will be given later. So plugging in: 
$$
|\frac{n}{n+1} - \frac{m}{m+1}| = |\frac{n(m+1)-m(n+1)}{(m+1)(n+1)}| = |\frac{n-m}{(m+1)(n+1)}|
$$
Assume that: $m \leq n$
$$
\leq|\frac{n}{(m+1)(n+1)}|
$$
$$
\frac{n}{n+1} < 1
$$
$$
\frac{1}{m+1} < \epsilon
$$
Proof:
Given $\epsilon > 0$ take $N$ such that $\frac{1}{N+1} < \epsilon$

Note: If $N \leq m \leq n$

We have 
$$
|\frac{1}{m+1}|<\epsilon
$$

From our initial calculations:
$$
|a_n - a_m| = |\frac{n}{n+1} - \frac{m}{m+1}| \leq |\frac{1}{m+1}| \leq |\frac{1}{N+1}| < \epsilon
$$

Theorem: $\{a_n\}^\infty_{n=1} \in R$ 
$a_n$ converges $\Leftarrow\Rightarrow$ $a_n$ is Cauchy
proof:
Suppose $\lim_{n\rightarrow\infty} a_n = L$ and we are given $\epsilon > 0$
Find $N \in \mathbb{N}$ such that if $n \geq N$ we have $|a_n - L| < \frac{\epsilon}{2}$