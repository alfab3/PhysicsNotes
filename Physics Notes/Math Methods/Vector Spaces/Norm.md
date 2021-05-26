A norm is a function $|| \cdot || V \rightarrow \mathbb{R}^+$ (non-negative reals) That satisfies

1) $||\lambda \vec{x}|| = |\lambda| ||\vec{x}||$
2) $||\vec{x} + \vec{y}|| \leq ||\vec{x}|| + ||\vec{y}||$ (triangle inequality) can also be written as:  $||\psi + \phi|| < ||\psi|| + ||\phi||$
3) $||\vec{x}|| = 0 \leftarrow \rightarrow \vec{x} = 0$

If 3 is not valid we call it a semiform.

Note: $\vec{x} = \ket{x}$

An inner product space ([[Inner Product Spaces]]) has a naturally defined norm 

$$||\vec{x}|| \equiv \sqrt{\braket{\vec{x},\vec{x}}}$$

or
  
$$||\psi|| = \braket{\psi | \psi}^{1/2}$$

In order to make $||\cdot ||_p$ a norm, we can restrict our space. We do so by declaring that a function like $f(x) = 1$ if $x = \frac{a + b}{2}$ and 0 otherwise. I will define this as equation $1$ 

More rigorously, we declare that two elements $f$ and $g$ of $F[a,b]$ are equivalent. $f \cong g$ if $||f - g|| = 0$

With this identification, the function 1 $\cong 0$ and our $F[a,b]$ with the above identification has now $||\cdot||_p$ as a norm.

This vector space is denoted as $L^p[a,b]$

In particular 
$$
||f||_2 = \sqrt{\braket{f,f}}
$$
where 
$$
\braket{f,g}:=\int_a^b f^\alpha (x)g(x)dx
$$
So that $L^2[a,b]$ is an inner product space


If you take ordinary vectors in $\mathbb{R}^3$ say, $\vec{a} \cdot \vec{b} = ab\cos{\theta}$. Where theta is the angle between them, and the magnitude of $\cos{\theta}$ is between -1 and 1. It follows that $|\vec{a}\cdot\vec{b}| \leq |\vec{a}||\vec{b}|$ Generalized $|\bra{\phi}\ket{\psi}|^2 \leq \bra{\phi}\ket{\phi}\bra{\psi}\ket{\psi}$ Cauchy-Schwartz inequality. When is this an equality or nonparallel. The equality iff $\ket{\phi} = a\ket{\psi}$. If $\phi$ is linearly dependent ([[Linear Independence]])on $\psi$ then the Cauchy-Schwartz inequality becomes an equality. 

