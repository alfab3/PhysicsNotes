If $a_{n+1}/a_n \leq r < 1$ for all sufficiently large $n$ and $r$ is independent of $n$,  the $\sum_n a_n$is convergent. If $a_{n+1}/a_n \geq 1$ for sufficiently large $n$ then $\sum_n a_n$ is divergent. 

This test is established by direct comparison with the geometric series $(1+r+r^2 + ...)$. In the second part, $a_{n+1} \geq a_n$ 

If:
$$
\lim_{n\to\infty} \frac{a_{n+1}}{a_n}
$$
$$
<1, convergence \;||
>1, divergence \; ||
=1, indeterminate
$$

Because of this final indeterminate possibility , the ratio test is likely to fail at crucial points.

Example :
Test $\sum_n\frac{n}{2}n$ for convergence. Applying the ratio test,
$$
\frac{a_{n+1}}{a_n} = \frac{(n+1)/2^{n+1}}{n/2^n} = \frac{1}{2}\frac{n+1}{n}
$$
Since 
$$
\frac{a_n+1}{a_n} \leq \frac{3}{4} \; \; n \geq 2
$$
we have convergence