Starting with [[Conservation of Angular Momentum in Polar Coordinates]], and integrating with respect to time. One will arrive at:

$$\begin{align} \theta(t) = \theta_0 +\frac{l}{m}\int^t_0\frac{dt'}{r^2(t')}\end{align}$$

Using the formula for [[Energy]]:

$$\begin{align} \frac{m\dot{x}^2}{2} + U(x) = E\end{align}$$

Solving for $\dot{x}$:
$$\begin{align} \dot{x} = \pm \sqrt{(2/m)[E-U(x)]} \end{align}$$

We arrive at [[Time Evolution of Two Body Problem]] specifically the integral: $$\begin{align}\sqrt{m/2}\int\frac{dr}{\sqrt{E-U_{eff}}} = \pm t \end{align}$$

Combining our theta integral with our t integral yields:

$$\begin{align} \theta = \pm \frac{l}{\sqrt{2m}} \int\frac{dr/r^2}{\sqrt{E - U_{eff}(r)}} \end{align}$$

and after some redimensionalization: $\rho = r/r_0$ and $\epsilon = E/|E_{min}|$ where $E_{min} = U_{eff}(r_0)$

For a potential of the form: $$-\frac{\gamma}{r^\alpha}$$
we get:
$$\begin{align} \theta = \pm \int \frac{d\rho/\rho^2}{\sqrt{(2-\alpha)\epsilon/a - 1/\rho^2+(2/\alpha)/\rho^\alpha}} \end{align}$$

or: 

$$\begin{align}|\theta_{p \to a}| = \pm \int^{\rho_p}_{\rho_a}\frac{d\rho/\rho^2}{\sqrt{(2-\alpha)\epsilon/a - 1/\rho^2+(2/\alpha)/\rho^\alpha}} \end{align}$$

Now for a potential of: $-\gamma/r$ i.e. $\alpha = 1$

When the integral is performed:
$$\begin{align}\theta = \pm arccos[(1/\rho)-1/\sqrt{1+\epsilon}] + \theta_0 \end{align}$$

Just set $\theta_0 = 0$ and solve:

$$\begin{align} \frac{1}{\rho} = 1 + \sqrt{1 + \epsilon} \cos\theta\end{align}$$

Which is a [[Conic Section]] with a focus at the origin.
