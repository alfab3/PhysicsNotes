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
Suppose $m,n \geq N$ and note
$$
|a_n - a_m| = |(a_n - L) + (L - a_m)|
$$
$$
|a_n - a_m| \leq |(a_n - L)| + |(a_m - L)| < \frac{\epsilon}{2}+\frac{\epsilon}{2} = \epsilon
$$

Now the other direction
Suppose $a_n$ is Cauchy
Part 1: Claim: $a_n$ is bounded

Take $N_1 \in \mathbb{N}$ such that $|a_m - a_n| < 1 \; \forall \; m,n \geq N$ 

Fix: $m = N_1 \Rightarrow \; |a_{N_1} - a_n| < 1 \;\forall \; n \geq N_1$
$$
\Rightarrow -1 < a_n - a_{N_1} < 1
$$
$$
\Rightarrow a_{N_1} - 1 < a_n < a_{N_1} + 1 
$$
$$
\Rightarrow |a_n| < |a_{N_1}| + 1 \; \; \forall \; n \geq N_1
$$
$$
|a_n| \leq max\{|a_1|, |a_2|, ... |a_{N_1 -1 }|, |a_{N_1} + 1 |\}
$$
$a_n$ is bounded

Find a convergent ([[Convergence]])  $\{a_{nk}\}^\infty_{k=1} \leq \{a_{n}\}^\infty_{n=1}$  
$$
\lim_{k\rightarrow\infty} a_{nk} = L
$$
Given $\epsilon >0$, 
take $k, N_2 \in \mathbb{N}$
$$
|a_{nk} - L| < \frac{\epsilon}{2}
$$
for all $k \geq K$
$$
|a_m - a_n| < \frac{\epsilon}{2}
$$
for all $m,n \geq N_2$
Suppose $n \geq N = max \{K, N_2\} ( n_k \geq N)$
$$
|a_{n} - L| \leq |a_{n} - a_{nk} + a_{nk} - L| \leq |a_{n} - a_{nk}| + |a_{nk} - L| < \epsilon
$$