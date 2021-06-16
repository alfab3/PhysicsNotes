Let f(x) be a continuous monotonic decreasing function in which $f(n) = a_n$. Then $\sum_n a_n$ converges if $\int^\infty_1 f(x)dx$ is finite and diverges if the integral is infinite. The $i$th partial sum is
$$
s_i = \sum^i_{n=1}a_n = \sum^i_{n=1} f(n)
$$
But, because $f(x)$ is monotonic decreasing, fig 1.1a [[series.png]]
$$
s_i \geq \int^{i+1}_1 f(x)dx
$$
On the other hand fig 1.1b [[series.png]]
$$
s_i-a_1 \leq \int^i_1f(x)dx
$$
Taking the limit as $i\rightarrow \infty$ we have
$$
\int^\infty_1 f(x)dx \leq \sum^\infty_{n=1} a_n \leq \int^\infty_1f(x)dx+a_1
$$
Hence the infinite series converges or diverges as the corresponding integral converges or diverges
This integral test is particularly useful in setting upper and lower bounds on the remainder of a series after some number of initial terms have been summed. That is, 
$$
\sum^\infty_{n=1} a_n = \sum^N_{n=1}a_n + \sum^N_{n=N+1}a_n
$$
and
$$
\int^\infty_{N+1}f(x)dx \leq \sum^\infty_{n=N+1} a_n\leq \int^\infty_{N+1}f(x)dx+a_{N+1}
$$
