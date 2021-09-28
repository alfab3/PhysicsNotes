$$\begin{align} f(x,y) = u(x,y) + iv(x,y)\end{align}$$ is a complex function where $u,v$ are real functions that satisfy the Cauchy-Riemann equations

Make variable transformation $x,y \rightarrow z(x,y),\bar{z}(x,y)$ and show:

$$\begin{align} \frac{\partial f(z,\bar{z})}{\partial\bar{z}} = 0 \end{align}$$

The Cauchy-Riemann equations show that: 
$$\begin{align} \frac{\partial u}{\partial x} = \frac{\partial v}{\partial y} \\ \frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x} \end{align}$$

Let: 
$$\begin{align} z =x + iy \\ \bar{z} = x -iy \end{align}$$

Using chain rule: 

$$\begin{align} \frac{\partial}{\partial x} = \frac{\partial z}{\partial x} \frac{\partial}{\partial z} + \frac{\partial \bar{z}}{\partial x} \frac{\partial}{\partial \bar{z}} \\ \frac{\partial z}{\partial x} =  \frac{\partial}{\partial x} (x +iy) = 1 \\ 
\frac{\partial \bar{z}}{\partial x} =\frac{\partial}{\partial x} (x -iy) = 1\\\frac{\partial }{\partial x} = \frac{\partial}{\partial z} + \frac{\partial}{\partial \bar{z}} \\
\\
\frac{\partial}{\partial y} = \frac{\partial z}{\partial y} \frac{\partial}{\partial z} + \frac{\partial \bar{z}}{\partial y} \frac{\partial}{\partial \bar{z}} \\ \frac{\partial z}{\partial y} =  \frac{\partial}{\partial y} (x +iy) = i \\ 
\frac{\partial \bar{z}}{\partial y} =\frac{\partial}{\partial y} (x -iy) = -i\\ \frac{\partial }{\partial y} = i\frac{\partial}{\partial z} - i \frac{\partial}{\partial \bar{z}} \end{align}$$

So now we have: $$\begin{align} \frac{\partial }{\partial x} = \frac{\partial}{\partial z} + \frac{\partial}{\partial \bar{z}} \\ \frac{\partial }{\partial y} = i(\frac{\partial}{\partial z} - \frac{\partial}{\partial \bar{z}})\end{align}$$

Plug into the Cauchy - Riemann equation:
$$\begin{align} \frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \;\frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x} \\ \left(\frac{\partial}{\partial z} + \frac{\partial}{\partial \bar{z}}\right)u = i\left(\frac{\partial}{\partial z} - \frac{\partial}{\partial \bar{z}}\right)v \\ i\left(\frac{\partial}{\partial z} - \frac{\partial}{\partial \bar{z}}\right)u = -\left(\frac{\partial}{\partial z} + \frac{\partial}{\partial \bar{z}}\right)v\end{align}$$

Now we have 2 unknowns and 2 equations so first solve for $\frac{dv}{dz}$ 

$$\begin{align} \frac{\partial u}{\partial z} + \frac{\partial u}{\partial \bar{z}} = i\frac{\partial v}{\partial z} - i  \frac{\partial v}{\partial \bar{z}} \\ i\frac{\partial z}{\partial z} = \frac{\partial u}{\partial z} + \frac{\partial u}{\partial \bar{z}}+i\frac{\partial v}{\partial \bar{z}} \\ \frac{\partial v}{\partial z} = \frac{1}{i} \left(\frac{\partial u}{\partial z} + \frac{\partial u}{\partial \bar{z}} \right) + \frac{\partial v}{\partial \bar{z}} \\  \frac{\partial v}{\partial z} = -i \left(\frac{\partial u}{\partial z} + \frac{\partial u}{\partial \bar{z}} \right) + \frac{\partial v}{\partial \bar{z}}\end{align}$$

Now we plug into the original equation:
$$\begin{align} i\frac{\partial u}{\partial z} - i \frac{\partial u}{\partial \bar{z}} = - \frac{\partial v}{\partial z} - \frac{\partial v}{\partial \bar{z}} \\ i\frac{\partial u}{\partial z} - i \frac{\partial u}{\partial \bar{z}} = i\frac{\partial u}{\partial z} + i \frac{\partial u}{\partial \bar{z}} - \frac{\partial v}{\partial z} - \frac{\partial v}{\partial \bar{z}} \\  - i \frac{\partial u}{\partial \bar{z}} = i \frac{\partial u}{\partial \bar{z}} - \frac{\partial v}{\partial z} - \frac{\partial v}{\partial \bar{z}} \\ -2i\frac{\partial v}{\partial \bar{z}}= 2\frac{\partial u}{\partial \bar{z}} \\ -i\frac{\partial v}{\partial \bar{z}}= \frac{\partial u}{\partial \bar{z}}\end{align}$$

So if we take the initial formula and perform a change of variables: $$\begin{align} f(x,y) = u(x,y) + iv(x,y) \rightarrow f(z,\bar{z}) = u(z,\bar{z}) + iv(z,\bar{z}) \end{align}$$

So differentiating with respect to $\bar{z}$ gives:
$$\begin{align} \frac{\partial f}{\partial \bar{z}} = \frac{\partial u}{\partial \bar{z}}+ i\frac{\partial v}{\partial \bar{z}}\end{align}$$

As shown above we proved that: $$\begin{align} i\frac{\partial v}{\partial \bar{z}}= -\frac{\partial u}{\partial \bar{z}} \end{align}$$
So the equation becomes: 
$$\begin{align} \frac{\partial f}{\partial \bar{z}} = \frac{\partial u}{\partial \bar{z}} - \frac{\partial u}{\partial \bar{z}} = 0\end{align}$$

The proof is complete.