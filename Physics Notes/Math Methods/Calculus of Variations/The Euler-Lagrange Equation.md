Suppose we gave differentiable function $J(y_1, y_2., ... y_n)$ of $n$ variables and seek its stationary points - these being the locations at which $J$ has its maxima, minima, and saddle points. At a stationary point $(y_1, y_2,...,y_n)$ the variation 

$$\delta J = \sum^n_{i=1} \frac{\partial J}{\partial y_i} \delta y_i$$

must be zero for all possible $\delta y_i$. The necessary and sufficient condition for this is that all partial derivatives $\partial J/\partial y_i,i=1,...,n$ be zero. By analogy, we expect that a functional([[Functional]]) $J[y]$ will be stationary under fixed-endpoint variations $y(x)\rightarrow y(x) + \delta y(x)$, when the functional derivative $\delta J/\delta y(x)$ vanishes for all x. In other words, when 

$$\frac{\partial f}{\partial y(x)} - \frac{d}{dx}(\frac{\partial f}{\partial y'(x)}) = 0, x_1 < x < x_2 $$

The condition for $y(x)$ to be a stationary point is usually called the Euler-Lagrange Equation. 

If the function $f$ depends on higher derivatives, $y'', y^{(3)}$, etc., then we have to integrate by parts more times and we end up with 

$$0 = \frac{\delta J}{\delta y(x)} = \frac{\partial f}{\partial y} - \frac{d}{dx}(\frac{\partial f}{\partial y'}) + \frac{d^2}{dx^2}(\frac{\partial f}{\partial y''}) - \frac{d}{dx^3}(\frac{\partial f}{\partial y^{(3)}})$$