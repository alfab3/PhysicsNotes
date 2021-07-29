Given the curve $y=x^2$ from $x = 0$ to $x=1$ find
a) the area under the curve (the area bounded by the curve the x-axis and the line $x=1$)
The area is $$\begin{align} A = \int^1_{x=0} ydx = \int^1_0x^2dx = \frac{x^3}{3}\bigg|^1_0=\frac{1}{3}\end{align}$$
We could also find the area as a double integral of $dA = dydx$ We have then $$\begin{align} A = \int^1_{x=0} \int^{x^2}_{y=0}dydx = \int^1_0x^2dx\end{align}$$

b) the mass of a plane sheet of material cut in the shape of this area if its density is $xy$
The element of area as in the double integral method in a is $dA = dydx$ Since the [[Density]] is $\rho = xy$ the element mass is $dM = xydydx$ and the total mass is $$\begin{align} M = \int^1_{x=0} \int^{x^2}_{y=0} xydydx = \int^1_0xdx\left[\frac{y^2}{2}\right]^{x^2}_0 = \int^1_0\frac{x^5}{2}dx=\frac{1}{12} \end{align}$$

c) the arc length of the curve 
the element of arc length $ds$ is defined as indicated thus we have:
$$\begin{align} ds^2 = dx^2 + dy^2 \\ ds = \sqrt{dx^2 + dy^2} = \sqrt{1+(dy/dx)^2}dx = \sqrt{(dx/dy)^2+1}dy \end{align}$$
If $y=f(x)$ has a continuous first derivative $dy/dx$ we can find the arc length of the curve $y=f(x)$ between $a$ and $b$ by calculating $\int^b_ads$ For our example we have $$\begin{align} \frac{dy}{dx} = 2x, \; \; ds = \sqrt{1+4x^2}dx \\ s = \int^1_0\sqrt{1+4x^2}dx=\frac{2\sqrt{5}+\ln(2+\sqrt{5})}{4} \end{align}$$

d) the centroid of the area
Recall from elementary physics that: 
The center of mass of a body has coordinates $\bar{x}, \bar{y}, \bar{z}$ given by the equation
$$\begin{align}\bar{x}dM = \int xdM \;\;\; \bar{y}dM = \int ydM \;\;\;\bar{z}dM = \int zdM\end{align}$$

The centroid of a body is the center of mass when we assume a constant density. In our example we have: $$\begin{align} \int^1_{x=0}\int^{x^2}_{y=0}\bar{x}dydx = \int^1_{x=0}\int^{x^2}_{y=0}xdydx \;\;\text{or}\;\; \bar{x}A=\frac{x^4}{4}\bigg|^1_0 = \frac{1}{4}\\ \int^1_{x=0}\int^{x^2}_{y=0} \bar{y} dydx = \int^1_{x=0}\int^{x^2}_{y=0} ydydx \;\;\text{or} \;\;\bar{y}A = \frac{x^5}{10}\bigg|^1_0=\frac{1}{10}\end{align}$$

e)the centroid of the arc
the center of mass $(\bar{x},\bar{y})$ of a wire bent in the shape of the curve $y=f(x)$ is given by 
$$\begin{align} \int\bar{x} \rho ds = \int x \rho ds \;\;\; \int \bar{y} \rho ds = \int y\rho ds\end{align}$$
where $\rho$ is the density (mass per unit length), and the integrals are single integrals with $ds$. If $\rho$ is constant the above equations defines the coordinates of the centroid. In our example we have 
$$\begin{align} \int^1_0\bar{x}\sqrt{1+4x^2}dx = \int^1_0x\sqrt{1+4x^2}dx\\
\int^1_0\bar{y}\sqrt{1+4x^2}dx = \int^1_0 y\sqrt{1+4x^2}dx = \int^1_0 x^2 \sqrt{1+4x^2}dx\end{align}$$

f) the momenta of inertia about the $x$, $y$, and $z$ xes of the lamina in $(b)$
The [[Moment of Inertia]] $I$ of a point mass $m$ about an axis is by definition the product $ml^2$ of $m$ times the square of the distance $l$ from $m$ to the axis. For an extended object we must integrate $l^2dM$ over the whole object, where $l$ is the distance from $dM$ to the axis.

In our example with variable density $\rho=xy$, we have $dM = xydydx$. The distance from $dM$ to the $x$ axis is $y$; similarly the distance from $dM$ to the $z$ axis is $\sqrt{x^2+y^2}$. Then the three moments of inertia about the three coordinate axes are:

$$\begin{align} I_x=\int^1_{x=0}\int^{x^2}_{y=0} y^2xydydx = \int^1_0 \frac{x^9}{4}dx=\frac{1}{40}\\ I_y = \int^1_{x=0}\int^{x^2}_{y=0} x^2xydydx=\int^1_0\frac{x^7}{2}dx=\frac{1}{16} \\ I_z = \int^1_{x=0}\int^{x^2}_{y=0}(x^2+y^2)xydydx =I_x+I_y=\frac{7}{80} \end{align}$$

The fact that $I_x + I_y$ = $I_z$ for a place lamina in the $(x,y)$ plane is known as the perpendicular axis theorem. 