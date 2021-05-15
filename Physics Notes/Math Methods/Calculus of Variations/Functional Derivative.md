We restrict ourselves to expressions of the form 
$$J[y] = \int^{x_2}_{x_1} f(x, y, y', y'', ..., y^{(n)})dx$$
where $f$ depends on the value of $y(x)$ and only finitely many of its [[Derivative]]. Such [[functionals]] are said to be local in $x$.

Consider first a functional $J = \int fdx$ in which $f$ depends only $x,y$ and $y'$. Make a change $y(x)\rightarrow y(x) + \epsilon \eta(x)$, where $\epsilon$ is a small $x$-independent constant. The resultant change in $J$ is

$$J[y+\epsilon\eta] - J[y] = \int_{x_1}^{x_2} \{f(x,y+\epsilon\eta,y' + \epsilon\eta') - f(x, y, y')\}dx = \int_{x_1}^{x_2} \{\epsilon \eta\frac{\partial f}{\partial y} +\epsilon \frac{d \eta}{dx}\frac{\partial f}{\partial y'} +O(\epsilon^2)\}dx$$

$$= [\epsilon \eta \frac{\partial f}{\partial y'}]^{x_2}_{x_1} + \int_{x_1}^{x_2} (\epsilon \eta(x)) \{\frac{\partial f}{\partial y} - \frac{d}{dx}(\frac{\partial f}{\partial y'})\} dx + O(\epsilon^2)$$

If $\eta(x_1) = \eta(x_2) = 0$ the variation $\delta y(x) \equiv \epsilon \eta(x)$ in $y(x)$ is said to have "fixed endpoints". For such variations the integrated-out part $[...]^{x_2}_{x_1}$ vanishes. Defining $\delta J$ to be the $O(\epsilon)$ part of $J[y + \epsilon \eta] - J[y]$, we have

$$\delta J = \int^{x_2}_{x_1}(\epsilon \eta(x))\{\frac{\partial f}{\partial y} - \frac{d}{dx}(\frac{\partial f}{\partial y'})\} dx = \int^{x_2}_{x_1} \delta y(x) (\frac{\delta J}{\delta y(x)})dx$$

The function 
$$\frac{\delta J}{\delta y(x)} \equiv \frac{\partial f}{\partial y} - \frac{d}{dx}(\frac{\partial f}{\partial y'})$$

is called the functional derivative of $J$ with respect to $y(x)$. We can think of it as a generalization of the partial derivative $\partial J/ \partial y_i$, where the discrete subscript $i$ on $y$ is replaced by a continuous label $x$ and sums over $i$ are replaced by integrals over $x$:

$$\delta J = \sum_i \frac{\partial J}{\partial y_i} \delta y_i \rightarrow \int^{x_2}_{x_1} dx (\frac{\delta J}{\delta y(x)}\delta y(x))$$