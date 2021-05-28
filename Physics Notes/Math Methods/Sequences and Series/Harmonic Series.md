Consider the harmonic series 
$$
\sum^\infty_{n=1} \frac{1}{n}=1+\frac{1}{2}+\frac{1}{3}+\frac{1}{4}+...+\frac{1}{n}+...
$$
The terms approach zero for large $n$ i.e., $\lim_{n\to\infty} 1/n =0$ but this is not sufficient to guarantee convergence. If we group the terms as 
$$
1 + \frac{1}{2}+(\frac{1}{3}+\frac{1}{4}) + ...
$$
each pair of parentheses encloses 
$$
\frac{1}{p+1} + \frac{1}{p+2} + ... + \frac{1}{p + p} > \frac{p}{2p} = \frac{1}{2}
$$
Forming partial sums by adding the parenthetical groups one by one, we obtain
$$
s_1 = 1, s_2 = \frac{3}{2}, s_3>\frac{4}{2}, s_4 >\frac{5}{2},...,s_n>\frac{n+1}{2}
$$
and we are forced to the conclusion that the harmonic series diverges.
