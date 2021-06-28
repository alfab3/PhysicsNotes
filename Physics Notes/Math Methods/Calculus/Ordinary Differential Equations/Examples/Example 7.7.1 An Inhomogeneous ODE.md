Consider the [[Ordinary Differential Equation]]
$$
(1-x)y''+xy' - y = (1-x)^2
$$
The corresponding homogeneous ODE has solutions $y_1 = x$ and $y_2 = e^x$. Thus, $y' =1$, $y'_2=e^x$ and the simultaneous equations for $u'_1$ and $u'_2$ are 
$$
xu'_1 + e^xu'_2 = 0
$$
$$
u'_1 + e^xu'_2 = F(x)
$$
Here $F(x)$ is the inhomogeneous term when the ODE has been written in the standard form. This means that we must divide the ODE through by $1-x$.

With the above choice $F(x)$, we solve the $u$ equations obtaining 
$$
u'_1 = 1, \; u'_2 = -xe^{-x}
$$
which integrate to $u_1 = x \; u_2 (x+1)e^{-x}$

Now forming a particular solution to the inhomogeneous ODE, we have 
$$
y_p(x)=u_1y_1 + u_2y_2 = x(x)+((x+1)e^{-x})e^x=x^2+x+1
$$

Because $x$ is a solution to the homogeneous equation, we may remove it from the above expression, leaving the more compact formula $y_p = x^2 +1$.

The general solution to our ODE therefore takes the final form 

$$
y(x) = C_1 x + C_2 e^x + x^2 + 1
$$