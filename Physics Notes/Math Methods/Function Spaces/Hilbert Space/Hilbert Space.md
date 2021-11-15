An [[Inner Product Spaces]] that is complete with respect to the norm $||\cdot|| = \sqrt{\braket{.,.}}$ is called the Hilbert space. 
$L^P[a,b]$ is Banach, $L^2[a,b]$ is Hilbert

Theorem: any inner product space $V$ has a unique completion $\bar{V}$ into a Hilbert space. (For instance $\mathbb{R} = \bar{\mathbb{R}}$)

Important example: if $C[a,b]$ is the vector space of all the continuous functions on $[a,b]$ with the inner product
$$\begin{align}
\braket{f,g} = \int^b_a f^\alpha(x)g(x)dx
\end{align}$$
then 
$$\begin{align}
\overline{C[a,b]} = L^2[a,b]
\end{align}$$