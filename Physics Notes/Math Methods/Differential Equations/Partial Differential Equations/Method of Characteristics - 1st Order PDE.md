It is useful to start study with properties of 1st order [[Partial Differential Equation]]s, for which we can always think as one variable (say x) as "space-like" and the second variable as "time-like"

The general form of 1st order linear PDE is:

$$\begin{gather} a(x,y)\frac{\partial u}{\partial x} + b(x,y)\frac{\partial u}{\partial y} + c(x,y) u = f(x,y) \\ y \to t \\ a(x,t)\frac{\partial u}{\partial x} + b(x,t)\frac{\partial u}{\partial t} + c(x,t) u = f(x,y)\end{gather}$$

Where $u(x,t)$ is the unknown [[Scalar Field]], $a(x,t), b(x,t), c(x,t)$ are known coefficients, f(x,t) is a known non-homogeneous source. 

As long as $a(x,t)$ and $b(x,t)$ don't vanish simultaneously (i.e. there is no $(x_0,t_0)$ such that $a(x_0,t_0) = b(x_0,t_0) = 0$) we can always introduce a family of curves (called characteristics) $[x_c,t_c]$ in the $(x,t)$ plane such that 
$$\begin{gather} \frac{dx_c}{ds} = a(x,t),\;\; \frac{dt_c}{ds} = b(x,t) \end{gather}$$

Which can be directly integrated to yield: 

$$\begin{gather} x_c(s) = x_0 + \int^S_{S'=0} a(x_c(s'),t_c(s'))ds' \\ y_c(s) = y_0 + \int^S_{S'=0} b(x_c(s'),t_c(s'))ds'\end{gather}$$
Families of characteristics are labeled by a parameter $c = (x_0,y_0)$, where $(x_0,y_0)$ could be any point a long a characteristic. 

![[characteristic curves 1.png]]

Characteristics are generally not parallel. Nevertheless, they don't intersect. This property follows from the linear nature of the PDE.

If the coefficients are constants then the characteristics are straight parallel lines of the form: $$\begin{gather}t_c(x) = t_0 + \frac{a}{b}x\end{gather}$$ alternatively:
$$\begin{gather} t_c(x) = t_0 +\frac{a}{b}(x-x_0) = (t_0 - \frac{a}{b}x_0)+\frac{a}{b}x\end{gather}$$
Demonstrating the parametric gauge nature of the parameter $c$.

The crucial point is that along any characteristic, the PDE reduces to an ODE. 
Namely noting that along the characteristic
$$\begin{gather} \frac{d u(s)}{ds} = \frac{dx_c}{ds}\frac{\partial u}{\partial x} + \frac{dt_c}{ds}\frac{\partial u}{\partial t}\\ \frac{dx_c}{ds} = a(x_c(s),t_c(s)) \\ \frac{dt_c}{ds} = b(x_c(s),t_C(s))\end{gather}$$

We obtain, along a characteristic, the ODE: 
$$\begin{gather} \frac{du}{ds} + c(s)u = f(s) \\ c(s) = c(x_c(s),t_c(s)) \\f(s) = f(x_c(s),t_c(s))\end{gather}$$

This is a 1st order ODE that can always be integrated out to give: 

$$\begin{gather} u(s)\equiv u[x_c(s),t_c(s)] \end{gather}$$

Hence with the method of characteristics we can solve exactly every 1st order PDE of the above type by plotting in the $x,t$ plane  plane a dense set of curves (characteristics) before attempting to solve the equation and then solve an ODE along each of these ($\infty$-many) curves.

Note that the method will fail if $a=b$ at a single point! Such a point similar to "caustic" is a focal point of multiple characteristics, such that contradicting information arrives from multiple sources.