Consider the ODE
$$
y'+\bigg(1+\frac{y}{x}\bigg)=0
$$
Multiplying by $xdx$, this ODE vecomes 
$$
(x+y)dx+xdy=0
$$
which is of the form 
$$
P(x,y)dx+Q(x,y)dy=0
$$
with $P(x,y) = x+y$ and $Q(x,y) = x$. The equation is not separable. To check if it is exact we compute
$$
\frac{\partial P}{\partial y}=\frac{\partial (x+y)}{\partial y}=1, \; \frac{\partial Q}{\partial x}=\frac{\partial x}{\partial x} = 1
$$
These partial derivatives are equal; the equation is exact and can be written in the form
$$
d\phi=Pdx + Qdy = 0
$$
The solution to the ODE will be $\phi = C$, with $\phi$ computed
$$
\phi = \int^x_{x_0} (x+y)dx + \int^y_{y_0}x_0dy = \bigg(\frac{x^2}{2} + xy - \frac{x_0^2}{2}- x_0y\bigg) + (x_0 y - x_0y_0)
$$
$$
=\frac{x^2}{2}+xy+constant \; terms
$$
Thus the solution 
$$
\frac{x^2}{2}+xy=C
$$