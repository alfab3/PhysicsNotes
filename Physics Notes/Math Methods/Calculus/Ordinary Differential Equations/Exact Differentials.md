We write the general [[Ordinary Differential Equation]] equation again
$$
P(x,y)dx+Q(x,y)dy=0
$$
This equation is said to be exact if we can match the left hand side of it to a differential $d\phi$ and thereby reach 
$$
d\phi=\frac{\partial\phi}{\partial x}dx + \frac{\partial \phi}{\partial y}dy =0
$$
Exactness therefore implies that there exists a function $\phi(x,y)$ such that
$$
\frac{\partial \phi}{\partial x} = P(x,y) \; and \; \frac{\partial \phi}{\partial y} = Q(x,y)
$$
Before seeking to find a function $\phi$ satisfying these equations, it is useful to determine whether such a function exists. Taking these two formulas differentiating the first with respect to $y$ and the second with respect to $x$
$$
\frac{\partial^2\phi}{\partial y \partial x}=\frac{\partial P(x,y)}{\partial y} \; and \; \frac{\partial^2\phi}{\partial x \partial y}=\frac{\partial Q(x,y)}{\partial x}
$$
and these are consistent if and only if
$$
\frac{\partial P(x,y)}{\partial y} = \frac{\partial Q(x,y)}{\partial x}
$$
The solution takes the form
$$
\phi(x,y)=\int^x_{x_0}P(x,y)dx + \int^y_{y_0}Q(x_0,y)dy=constant
$$
