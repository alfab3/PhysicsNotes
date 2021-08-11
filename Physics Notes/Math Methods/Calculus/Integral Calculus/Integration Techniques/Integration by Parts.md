A helpful method for integration when the [[Integral]] consists of two functions multiplied by each other. The general form:
$$\begin{align} \int uv \;dx = u\int v dx - \int u' (\int v \; dx)dx\end{align}$$

Where: $u$ is the function $u(x)$, $v$ is the function $v(x)$, and $u'$ is the derivative of the function $u(x)$. 

Example: 
Solve $$\begin{align}\int x\cos(x)\; dx \end{align}$$

First choose which functions for $u$ and $v$: $$\begin{align} u=x \\v = \cos(x)\end{align}$$

Differentiate: $u$: $u' = x' = 1$, integrate $v$: $\int v \;dx = \cos(x)\;dx = \sin(x)$

Now put it together: 
$$\begin{align} \int x \cos(x) \; dx = x \sin(x) - \int1(\sin(x))dx \\= x sin(x) - \int\sin(x)\; dx \\ = x\sin(x)+\cos(x)+C\end{align}$$

Another form may look like: 
$$\begin{align} \int udv = uv - \int v\;du \end{align}$$