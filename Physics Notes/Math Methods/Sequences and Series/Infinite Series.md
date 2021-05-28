Fundamental Concepts
The usual way of assigning a meaning to the sum of an infinite number of terms is by introducing the notion of partial sums. If we have an infinite sequence of terms $u_1, u_2, u_3, u_4, u_5,...,$ we define the $i$th partial sum as 

$$
s_i = \sum^i_{n=1} u_n
$$

This is a finite summation and offers no difficulties. If the partial sums $s_i$ converge to a finite limit as $i \rightarrow \infty$
$$
\lim_{i \rightarrow \infty} s_i = S
$$

the infinite series $\sum^i_{n=1} u_n$ is said to be convergent and to have the value $S$. Note that we define the infinite series as equal to $S$ and that a necessary condition for convergence to a limit is that that $\lim_{n\rightarrow\infty} u_n =0$. This condition however is not sufficient to guarrantee convergence.

Sometimes it is convenient to apply the condition in the limit in a form called the Cauchy Criterion, ([[Cauchy Sequences]]).

Some series diverge, meaning that the sequence of partial sums approaches $\pm\infty$; others may have partial sums that oscillate between two values, as for example:
$$
\sum^\infty_{n=1} u_n = 1 - 1 + 1 - 1 - ... -(-1)^n+...
$$
The series does not converge and can be called oscillatory.