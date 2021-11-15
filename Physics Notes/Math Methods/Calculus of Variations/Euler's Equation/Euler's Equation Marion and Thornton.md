The condition that the integral of a [[Functional]] has an extremum requires a formula such that the Functional has a maximum or minimum value.

Assume we are looking for some function $y(x)$ such that the integral:

$$\begin{align} J = \int^{x_b}_{x_a}f\{y(x),\ y'(x);\ x\} dx\end{align}$$

is an extremum (min or max).The points $x_a$ and $x_b$ are fixed.

The function $y(x)$ is to be varied until an extreme value of $J$ is found. (If a function $y(x)$ gives a minimum value then any neighboring function must make $J$ increase). The definition for a neigboring function is then written as:

$$\begin{align} y(\alpha,x) = y(0,x) + \alpha \eta(x)\end{align}$$

Where $\eta(x)$ is some function of $x$ that has a continuous first [[Derivative]] and that vanishes at $x_1$ and $x_2$ since the varied function $y(\alpha,x)$ must be identical to $y(x)$ at the endpoints of the path: $\eta(x_1) = \eta(x_2)= 0$

Now rewrite the integral with the new parameter:

$$\begin{align} J(\alpha) = \int^{x_2}_{x_1} f\{y(\alpha, x),\ y'(\alpha,x); \ x\} dx\end{align}$$

The conditon that the integral have a stationary value is that $J$ be independent of $\alpha$ in first order along the path giving the extrenum $(\alpha = 0)$ or equivalently that $$\begin{align}\frac{\partial J}{\partial \alpha}\Bigg|_{\alpha=0} = 0\end{align}$$

For all functions of $\eta(x)$

Now lets plug in our integral:

$$\begin{align} \frac{\partial J}{\partial \alpha} = \frac{\partial}{\partial \alpha} \int^{x_2}_{x_1} f\{y, y', x\} dx\end{align}$$

The differential operation affects only the integrand:

$$\begin{align} \frac{\partial J}{\partial \alpha} = \int^{x_2}_{x_1}\left(\frac{\partial f}{\partial y} \frac{\partial y}{\partial \alpha} + \frac{\partial f}{\partial y'} \frac{\partial y'}{\partial \alpha}\right)dx\end{align}$$

Then from the definition of the neighbor function:
$$\begin{align} \frac{\partial y}{\partial \alpha}  = \eta(x); \; \frac{\partial y'}{\partial \alpha} = \frac{d\eta}{d x}\end{align}$$

Plugging in these values to our integrand gives us:

$$\begin{align}\frac{\partial J}{\partial \alpha} = \int^{x_2}_{x_1}\left(\frac{\partial f}{\partial y} \eta(x) + \frac{\partial f}{\partial y'} \frac{d \eta}{d x}\right)dx \end{align}$$

The second term in the integrand can be solved by [[Integration by Parts]]:

$$\begin{align} \int^{x_2}_{x_1}\frac{\partial f}{\partial y'}\frac{d\eta}{dx}dx = \frac{\partial f}{\partial y'}\eta(x)\Bigg|^{x_2}_{x_1} - \int^{x_2}_{x_1}\frac{d}{dx}\left(\frac{\partial f}{\partial y'}\right)\eta(x)dx\end{align}$$

The first term vanishes becuase of the boundary conditions $\eta(x_1) = \eta(x_2) = 0$ 

Now we can easily see that: 

$$\begin{gather} \frac{\partial J}{\partial \alpha} = \int^{x_2}_{x_1} \left[\frac{\partial f}{\partial y} \eta(x) - \frac{d}{dx}\left(\frac{\partial f}{\partial y'}\right)\eta(x)\right] dx \\ = \int^{x_2}_{x_1}\left(\frac{\partial f}{\partial y}- \frac{d}{dx}\frac{\partial f}{\partial y'}\right) \eta(x) dx\end{gather}$$

The integral appears to be independent of $\alpha$. But the functions $y$ and $y'$ with respect to which the derivatives of $f$ are taken are still functions of $\alpha$. Because $(\partial f/\partial \alpha)|_{\alpha=0}$ must vanish for the extremum value and because $\eta(x)$ is an arbitrary function the integrand in must vanish for $\alpha = 0$:

$$\begin{align} \frac{\partial f}{\partial y} - \frac{d}{dx}\frac{\partial f}{\partial y'} = 0\end{align}$$

Which is Euler's Equation.

where $y$ and $y'$ are the original functions, independent of $\alpha$. 