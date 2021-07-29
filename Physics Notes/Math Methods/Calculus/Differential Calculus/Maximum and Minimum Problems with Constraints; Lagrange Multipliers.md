A wire is bent to fit the curve $y=1-x^2$. A string is stretched from the origin to a point $(x,y)$ on the curve. Find $(x,y)$ on the curve. Find $(x,y)$ to minimize the length of the string. 

We want to minimize the distance $d=\sqrt{x^2+y^2}$ from the origin to the point $(x,y)$; this is equivalent to minimizing $f = d^2 = x^2+y^2$. But $x$ and $y$ are not independent; they are related by the equation of the curve. This extra relation between the variables is what we mean by a constraint. Problems involving constraints occur frequently in applications. 

There are several methods to do a problem like this:
a) Elimination
The most obvious method is to eliminate $y$. Then we want to minimize $$\begin{align} f = x^2 + (1-x^2)^2= x^2+1-2x^2=x^4-x^2+1\end{align}$$

This is just an ordinary calculus problem:
$$\begin{align} \frac{df}{dx} = 4x^3 - 2x = 0, \;\; x=0 \;\;\; \text{or} \;\;\; x = \pm\sqrt\frac{1}{2}\end{align}$$

It is not immediately obvious which of these points is a maximum and which is a minimum, so in this simple problem it is worth while to find the second derivative:
$$\begin{align} \frac{d^2f}{dx^2}=12x^2-2 =\begin{cases} -2 &\text{at}& x = 0\\ 4 & \text{at} & x=\pm\sqrt{1/2}\end{cases}\end{align}$$

b) Implict Differentiation
Suppose it had not been possible to solve for $y$ and substitute; we could still do the problem. From $f = x^2 + y^2$ we find $$\begin{align} df = 2xdx + 2ydy \;\;\; \text{or} \;\;\; \frac{df}{dx} = 2x + 2y\frac{dy}{dx}\end{align}$$

From an equation like $y = 1-x^2$ relating $x$ and $y$, we could find $dy$ in terms of $dx$ even if the equation were not solvable for $y$. Here we get
$$\begin{align} dy=-2xdx \end{align}$$
Eliminating $dy$ from $df$ we have $$\begin{align} df = (2x-4xy)dx \;\;\; \text{or} \;\;\; \frac{df}{dx}=2x-4y\end{align}$$
To minimize $f$ we set $df/dx=0$. This gives $2x-4xy = 0$. This equation must now be solved simultaneously with the equation of the curve $y=1-x^2$. We get $2x-4x(1-x^2)=0,x=0\; \text{or}\;\pm\sqrt{1/2}$ as before. To test maxima or minima we need $d^2f/dx^2$. Differentiationg $df/dx$ with respect to $x$ we get
$$\begin{align} \frac{d^2f}{dx^2} = 2 + 2\left(\frac{dy}{dx} \right)^2 +2y\frac{d^2y}{dx^2}\end{align}$$
At $x=0$, we find $y=1$, $dy/dx=0$, $dy^2/dx^2 = -2$, so 
$$\begin{align}\frac{d^2f}{dx^2} = 2 -4 =-2\end{align}$$
this is a maximum point. At $x=\pm\sqrt{1/2}$ we find 
$$\begin{align} y = \frac{1}{2}, \; \frac{dy}{dx}= \mp\sqrt{2}, \frac{d^2y}{dx^2}=-2\end{align}$$
so
$$\begin{align}\frac{d^2f}{dx^2} = 2 + 4 - 2 =4 \end{align}$$
this point is the required minimum. 

c)Lagrange Multipliers
Methods a and b can involve an enormous amount of algebra. We can shortcut this algebra by a process known as the method of Lagrange multipliers or undetermined multipliers. We want to consider a problem like the one we discussed in a or b. In general we want to find the maximum or minimum of a function $f(x,y)$, where $x$ and $y$ are related by an equation $\phi(x,y) =$ const. Then $f$ is really a function of one variable say $x$. To find maximum or minimum points of $f$, we set $df/dx = 0$ or $df = 0$. Since $\phi =$ const., we get $d\phi = 0$
$$\begin{align}df =\frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy = 0 \\ d\phi = \frac{\partial \phi}{\partial x}dx + \frac{\partial \phi}{\partial y}dy = 0 \end{align}$$

To find the maximum or minimum values of $f(x,y)$ when $x$ and $y$ are related by the equation $\phi(x,y)=$ const. form the function $F(x,y)$ as in $F(x,y)=f(x,y)+\lambda\phi(x,y)$ and set the two partial derivatives of $F$ equal to zero $\frac{\partial f}{\partial y} + \lambda\frac{\partial \phi}{\partial y} = 0$ and $\frac{\partial f}{\partial x} + \lambda\frac{\partial \phi}{\partial x} = 0$. Then solve these two equations and the equation $\phi(x,y) =$ const for the three unknowns $x$,$y$, and $\lambda$