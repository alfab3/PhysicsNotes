Let f(x) be a continuous monotonic decreasing function in which $f(n) = a_n$. Then $\sum_n a_n$ converges if $\int^\infty_1 f(x)dx$ is finite and diverges if the integral is infinite. The $i$th partial sum is
$$
s_i = \sum^i_{n=1}a_n = \sum^i_{n=1} f(n)
$$
But, because $f(x)$ is monotonic decreasing, 
$$
s_i \geq \int^{i+1}_1 f(x)dx
$$
On the other hand 
$$
s_i-a_1 \leq \int^i_1f(x)dx
$$
