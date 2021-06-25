Consider the linear classical oscillator [[Harmonic Oscillator]] equation 
$$
\frac{d^2y}{dx^2}+\omega^2 y = 0
$$
The solutions are $y=\sin\omega x$ and $y = \cos \omega x$ found in [[Example 7.3.1 Hooke's Law Spring]]

We try 
$$
y(x)=x^s(a_0+a_1x+a_2x^2+a_3x^3 + \dots) = \sum^ \infty_{j=0} a_jx^{s+j}
$$
with the exponent $s$ and all the coefficients $a_j$ still undetermined. Note that $s$ need not be an integer. By differentiating twice we obtain 
$$
\frac{dy}{dx}=\sum^\infty_{j=0} a_j(s+j)x^{s+j-1}
$$
$$
\frac{d^2y}{dx^2}=\sum^\infty_{j=0} a_j(s+j)(s+j-1)x^{s+j-2}
$$
By substituing this into our oscillator equation we get
$$
\sum^\infty_{j=0}a_j(s+j)(s+j-1)x^{s+j-2}+\omega^2\sum^\infty_{j=0} a_j x^{s+j}=0
$$

The coefficient of each power of x on the left-hand side of the equation must vanish individually, $x^s$ being an overall factor. 

The lowest power of $x$ appearing in the equation is $x^{s-2}$, occuring only for $j=0$ in the first summation. The requirement that ihis coeeficient vanish yields
$$
a_0s(s-1)=0
$$
Recall that we chose $a_0$ as the coefficient of the lowest nonvanishing term of the series 
$$
y(x)=x^s(a_0+a_1x+a_2x^2+a_3x^3 + \dots) = \sum^ \infty_{j=0} a_jx^{s+j}
$$
so that by definition $a_0 \neq 0$. Therefore we have
$$
s(s-1)=0
$$
This equation, coming from the coefficient of the lowest power of $x$, is called the indicial equation. The indicial equation and its roots are of critical importance to our analysis. Clearly, in this example  it informs us that either $s=0$ or $s=1$ so that our series solution must start either with an $x^0$ or an $x^1$ term.

