If term by term a series of terms $u_n$ satisfies $0 \leq u_n \leq a_n$, where the $a_n$ form a covergent series, then the series $\sum_n u_n$ is also convergent. Letting $s_i$ and $s_j$ be partial sums of the $u$ series, with $j > i$, the difference $s_j - s_i$ is $\sum^j_{n = i + 1} u_n$, and this is smaller than the corresponding quantity for the a series, thereby proving convergence. A similar argument shows that if term by term a series of terms $v_n$ satisfies $0 \leq b_n \leq v_n$ where the $b_n$ form a divergent series, then $\sum_n v_n$ is also divergent. 
For the convergent series $a_n$ we already have the geometric series, whereas the harmonic series will serve as the divergent comparison series $b_n$. As other series are identified as either covergent or divergent, they may also be used as the known series for comparison. 

Example
Test $\sum^\infty_{n=1} n^{-p}$, $p = 0.999$ for convergence. Since $n^{-0.999} > n^{-1}$ and $b_n = n^{-1}$ forms the divergent harmonic series, the comparison test shows that $\sum_n n^{-0.999}$ is divergent. Generalizing $\sum_n n^{-p}$ is seen to be divergent for all $p \leq 1$