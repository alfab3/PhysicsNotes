Find the colume of the solid below the plave $z = 1 + y$ bounded by the coordinate planes and the vertical plane $2x+y=2$.  This is $\int \int_A zdxdy = \int\int_A (1+y)dxdy$ where $A$ is the triangle in the $x,y$ plane created by $2x+y=2$ To determine the volume we must first integrate with respect to $y$ and keep $x$ constant from $y=0$ to $y$ on the line $2x+y=2$ that is $y = 2 -2x$; we find$$\begin{align} \int^{2-2x}_{y=0} z dy = \int^{2-2x}_{y=0} (1+y)dy = \left(y + \frac{y^2}{2}\right)\bigg|^{2-2x}_0 \\ = (2-2x)+(2-2x)^2/2 = 4 - 6x +2x^2 \end{align}$$ Now we integrate with respect to $x$ $$\begin{align} \int^1_{x=0}(4-6x+2x^2)dx = \frac{5}{3}\end{align}$$

This can also be written as:
$$\begin{align} \int_{x=0}^1\int^{2-2x}_{y=0} zdydx = \int_{x=0}^1\int^{2-2x}_{y=0} (1+y)dydx  \end{align}$$
and so on.

