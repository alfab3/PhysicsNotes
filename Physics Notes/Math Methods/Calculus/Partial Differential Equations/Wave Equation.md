$$\begin{align} \frac{d^2u}{dx^2} = \frac{1}{c^2}\frac{\partial^2u}{\partial t^2}\end{align}$$

1st order PDE's

$$\begin{align} a(x,t)\frac{\partial u}{\partial x} +b(x,t)\frac{\partial u}{\partial t}+c(x,t)u=f(x,t)\end{align}$$

Where a, b, c are coefficients and $f(x,t)$ is a non-homogeneous source

Our purpose is to find the value of $u(x,t)$ at any point $x$ and $t$.

Any curve on the $x - t$ plane are called a characteristic curve. Which are related to the formula not the solution.

What is the equation of the curve in the $x-t$ plane?

$$\begin{align} [x_c(s), t_c(s)]\end{align}$$

Where $c$ is a label of the characteristic, each c signifies a different line.

Characteristic family - set of [[Characteristic Curves]] that populate a plane.

$$\begin{align} \frac{dx_c(s)}{ds} = a[x_c(s),t_c(s)] \\\frac{dt_c(s)}{ds} = b[x_c(s),t_C(s)] \\ x_c(s) = x_0 + \int^S_{S=0}a[x_c(s'),t_c(s')]ds' \\ t_c(s) = t_0 + \int^S_0b[x_c(s'),t_c(s')]ds' \end{align}$$

$$\begin{align} u_c(s) \equiv u_c[x_c(s), t_c(s)] \\ \frac{du_c}{ds} = \frac{dx_c}{ds}\frac{\partial u}{\partial x} + \frac{dt_c}{ds}\frac{\partial u}{\partial t}\\ \frac{du}{ds} +C(s)\cdot u_c(s) = f(s)\end{align}$$

Where $c(s) = c[x_c(s),t_c(s)]$ and $f(s) = f[x_c(s),t_c(s)]$

$$\begin{align} \frac{dt_c}{dx_c} = \frac{b(x_c,t_c)}{a(x_c,t_c)} \end{align}$$

if $a=a_0$, $b = b_0$

$$\begin{align}x_c(S) = x_0 + as\\ y_c(s) = y_0 +bs \\ t_c(x) = t_0 +\left(\frac{b_0}{a_0}\right)(x-x_0) \\ c = t_0 - \frac{b_0}{a_0}x_0\end{align}$$

