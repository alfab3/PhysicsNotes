Consider a linear, second-order, homogeneous [[Ordinary Differential Equation]] in the form:
$$
\frac{d^2y}{dx^2}+P(x)\frac{dy}{dx}+Q(x)y=0
$$
In this section we develop (at least) one solution of this equation by expansion about the point $x=0$. In the next section we develop the second, independent solution and prove that no third independent solution exists. Therefore the most general solution may be written in terms of the two independent solutions as 
$$
y(x)=c_1y_1(x)+c_2y_2(x)
$$
Our physical problem may lead to a nonhomogeneous, linearm second-order ODE
$$
\frac{d^2y}{dx^2}+P(x)\frac{dy}{dx}+Q(x)y=F(x)
$$
The function on the right $F(x)$, typically represents a source or a driving force. 

Assuming a single particular integral, $y_p$ of the inhomogeneous ODE to available, we may add to it any solution of the corresponding homogeneous equationg and write the most general solution 
$$
y(x)=c_1y_1(x) + c_2y_2(x) + y_p(x)
$$
In many problems, the constants $c_1$ and $c_2$ will be fixed by boundary conditions.