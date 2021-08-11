Derive the [[Law of reflection]]. Hint: Let light go from the point $A=(x_1,y_1)$ to $B=(x_2,y_2)$ via an arbitrary point $P = (x,0)$ on a mirror along the x axis. Set $dt/dx=(n/c)dD/dx = 0$ where $D$ = distance $APB$. Show then that $\theta = \phi$. 

[[Fermat's Principle]]: Light follows the path of least time. 

![[problem 9.1 figure.png]]

The pathlength from $A\; \text{to} \; B$ is:
$$\begin{align} L = \sqrt{a^2+b^2} + \sqrt{b^2+(d-x)^2}\end{align}$$

Where $d$ is the distance between the two points on the x-axis and x is the distance between the middlepoint and point A.

Since the speed is constant the minimum time path is simply the minimum distance path. This may be found by setting the derivative of $L$ with respect to $x$ equal to zero. 
$$\begin{align} \frac{dL}{dx} = \frac{1}{2}\frac{2x}{\sqrt{a^2+x^2} }+ \frac{(d-x)(-1)}{\sqrt{b^2+(d-x)^2}} \\ \sin\theta = \sin\phi\end{align}$$

Heres the more complicated way to do it:

$$\begin{align} t = \int_A^B dt \\ = c^{-1}\int^B_A nds \\  = c^{-1}n\int^B_A ds \\ = c^{-1} n (AP+PB) \\ = c^{-1}n\left(\sqrt{(x-x_1)^2 + (0 - y_1)^2} + \sqrt{(x_2-x)^2+(y_2-0)^2}\right) \\ = c^{-1} n \left(\sqrt{(x-x_1)^2 + y_1^2} + \sqrt{(x_2-x)^2+y_2^2} \right) \end{align}$$

According to Fermat's principle the time of travel is stationary so: 
$$\begin{align} \frac{dt}{dx} = 0 \\ \frac{d}{dx}\left[ c^{-1}n\left( \sqrt{(x-x_1)^2 + y_1^2} + \sqrt{(x_2-x)^2+y_2^2} \right) \right] = 0 \\ \frac{2(x-x_1)}{2\sqrt{(x-x_1)^2+y_1^2}} + \frac{-2(x_2-x)}{2\sqrt{(x_2-x)^2+y_2^2}} = 0 \\ \frac{(x-x_1)}{\sqrt{(x-x_1)^2}+y_1^2} = \frac{(x-x_1)}{\sqrt{(x-x_2)^2}+y_2^2} \\ \sin\theta = \frac{(x-x_1)}{\sqrt{(x-x_1)^2}+y_1^2}, \;\; \sin \phi = \frac{(x-x_2)}{\sqrt{(x-x_2)^2}+y_2^2}\\ \sin\theta = \sin\phi \\ \theta=\phi\end{align}$$