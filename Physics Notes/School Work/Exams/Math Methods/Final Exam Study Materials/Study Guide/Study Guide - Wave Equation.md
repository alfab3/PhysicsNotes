# Definition
[[Hyperbolic Equations]] that has solution $\varphi(x,t)$ which obeys the wave equation:

$$\begin{gather} \frac{\partial^2 \varphi}{\partial x^2} - \frac{1}{c^2}\frac{\partial^2\varphi}{\partial t^2} = 0\end{gather}$$

# Solutions
### D'Alembert's Solution
$$\begin{gather} \phi(x,t) = \frac{1}{2}\{\varphi_0(x+ct, 0) +  \varphi_0(x-ct),0\} + \frac{1}{2c}\int^{x+ct}_{x-ct}v_0(\xi)d\xi \end{gather}$$

Where:

$$\begin{gather} \varphi_0 = \varphi(x,t=0) \\ 
v_0 = \frac{\partial \varphi}{\partial t}(x,t=0)\end{gather}$$

### Green's Function

The [[Green's Function]] of the [[Wave Equation]] is: 

$$\begin{gather}G(x-x_0,t-t_0) = \frac{1}{2c}\{H(x-x_0+c(t-t_0))-H(x-x_0 -c(t-t_0))\} \end{gather}$$

Where $H$ is the Heaviside function


