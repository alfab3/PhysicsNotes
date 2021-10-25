in [[Euler's Equation]] we defined the integral to find the extremum as:

$$\begin{align} \frac{\partial J}{\partial \alpha} d\alpha = \int^{x_2}_{x_1}\left(\frac{\partial f}{\partial y} - \frac{d}{dx}\frac{\partial f}{\partial y'}\right)\frac{\partial y}{\partial \alpha} d\alpha dx\end{align}$$

This may be expressed as: 

$$\begin{align} \delta J = \int^{x_2}_{x_1}\left(\frac{\partial f}{\partial y} - \frac{d}{dx}\frac{\partial f}{\partial y'}\right) \delta y dx \end{align}$$

where:

$$\begin{align} \frac{\partial J}{\partial \alpha} d\alpha \equiv \delta J \\ \frac{\partial y}{\partial \alpha}d\alpha \equiv \delta y \end{align}$$

The condtion of extremum then becomes $$\begin{align} \delta J = \delta \int^{x_2}_{x_1} f\{y,y';x\}dx = 0\end{align}$$

Which when solving gives us:

$$\begin{align} \delta J = \int^{x_2}_{x_1} \left(\frac{\partial f}{\partial y} - \frac{d}{dx}\frac{\partial f}{\partial y'}\right)\delta y dx\end{align}$$