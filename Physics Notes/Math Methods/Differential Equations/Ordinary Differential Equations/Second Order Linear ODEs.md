Singular Points

The concept of singularity of an [[Ordinary Differential Equation]] is important to us for two reasons: (1) it is useful for classifying ODEs and identifying those that can be transformed into common forms, and (2) it bears on the feasibility of finding series solutions to the ODE.

When a linear homogeneous second order ODE is written in the form
$$
y''+P(x)y'+Q(x)y=0
$$
points $x_0$ for which $P(x)$ and $Q(x)$ are finite are termed ordinary points of the ODE. However, if either $P(x)$ or $Q(x)$ diverge as $x\rightarrow x_0$, the point $x_0$ is called a singular point. Singular points are further classified as regular or irregular.

A singular point $x_0$ is regular if either $P(x)$ or $Q(x)$ diverges there, but $(x-x_0)P(x)$ and $(x-x_0)^2Q(x)$ remain finite

A singular point $x_0$ is irregular if $P(x)$ diverges faster thatn $1/(x-x_0)$ so that $(x-x_0)P(x)$ goes to infinity as $x \rightarrow x_0$, or if $Q(x)$ diverges faster than $1/(x-x_0)^2$ so that $(x-x_0)^2Q(x)$ goes to infinity as $x \rightarrow x_0$

These definitions hold for all finite values of $x_0$. To analyze the behavior at $x\rightarrow \infty$ we set $x=1/z$, substitute into the differential equation, and examine the behavior in the limit $z\rightarrow 0$. The ODE, originally in the dependent variable $y(x)$, will now be written in terms of $w(z)$, defined as $w(z)=y(z^{-1})$. Converting the [[Derivative]]
$$
y'=\frac{dy(x)}{dx}=\frac{dy(z^{-1})}{dz}\frac{dz}{dx}=\frac{dw(z)}{dz}\bigg(-\frac{1}{x^2}\bigg)=-z^2w'
$$
$$
y''=\frac{dy'}{dz}\frac{dz}{dx}=(-z^2)\frac{d}{dz}[-z^2 w'] = z^4w'' + 2z^3w'
$$

Plugging in to our original equation
$$
z^4w'' + [2z^3 - z^2P(z^{-1})]w' + Q(z^-1)w = 0
$$
Dividing through by $z^4$ to place the ODE in standard form, we see that the possibility of a singularity at $z=0$ depends on the behavior of 
$$
\frac{2z-P(z^{-1})}{z^2} \; and \; \frac{Q(z^{-1})}{z^4}
$$
If these two expressions remain finite at $z=0$, the point $x=\infty$ is an ordinary point. If they diverge no more rapidly than $1/z$ and $1/z^2$, respectively, $x=\infty$ is a regular singular point otherwise it is an irregular singular point. 