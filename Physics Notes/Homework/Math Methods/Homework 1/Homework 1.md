Albert Fabrizi

Problem 1

2 pairs of real numbers: $(x_1,y_1),(x_2,y_2)$ 

$\vec{a_k} = x_k \hat{i} + y_k \hat{j}$ and $a_k = x_k + iy_k$ for $k=1,2$

Prove: $$\begin{align}\vec{a}_1\cdot\vec{a}_2 = \frac{1}{2}(a_1\bar{a}_2 + \bar{a}_1 a_2) \end{align}$$

Left hand side:
$$\begin{align} \vec{a}_1\cdot\vec{a}_2 = (x_1 \hat{i} + y_1 \hat{j}) \cdot (x_2 \hat{i} + y_2 \hat{j}) = (x_1x_2 + y_1y_2) \end{align}$$

Right hand side:

$$\begin{align} \frac{1}{2}(a_1\bar{a}_2 + \bar{a}_1 a_2) = \frac{1}{2}[(x_1+iy_1)(x_2-iy_2) +(x_1 - iy_2)(x_2+iy_2)] \\ = \frac{1}{2}[(x_1x_2 - iy_2x_1 + iy_1x_2 + y_1y_2)+ (x_1x_2 + iy_2x_1 - iy_1x_2+y_1y_2)] \\ = \frac{1}{2}[(x_1x_2 + y_1y_2 + x_1x_2 + y_1y_2 - iy_2x_1 + iy_2x_1 + iy_1x_2 - iy_1x_2)] \\= \frac{1}{2}[(x_1x_2+y_1y_2+x_1x_2 + y_1y_2 - 0)] \\ = \frac{1}{2}[(x_1x_2+y_1y_2 + x_1x_2 + y_1y_2)] = \frac{1}{2}[2(x_1x_2+y_1y_2)] =(x_1x_2+y_1y_2) \end{align}$$

Therefore plugging in both left hand and right hand side: 
$$\begin{align} (x_1x_2 + y_1y_2) = (x_1x_2 + y_1y_2)\end{align}$$

The proof is complete.

Now prove: $$\begin{align} \vec{a_1} \times \vec{a_2} \cdot \hat{z} = \frac{i}{2}(a_1\bar{a}_2 - \bar{a}_1a_2)\end{align}$$

Left hand side:

$$\begin{align} (x_1 \hat{i} + y_1\hat{j}) \times (x_2 \hat{i} + y_2\hat{j}) \cdot \hat{z}\end{align}$$

Solve the cross product: 
$$\begin{align} \begin{bmatrix} \hat{i} &\hat{j} &\hat{z} \\ x_1 & y_1 & 0 \\ x_2 & y_2 & 0 \end{bmatrix}  = \hat{i}(0-0) + \hat{j}(0-0) + \hat{z}(x_1y_2 - y_1x_2)\end{align}$$

Plug back in to left hand side:
$$\begin{align} \text{The unit vectors cancel: } (\hat{z}\cdot\hat{z} = 1) \\ (x_1y_2 - y_1x_2)\hat{z} \cdot \hat{z} = (x_1y_2 - y_1x_2) \end{align}$$

Now the Right hand side:

$$\begin{align} \frac{i}{2}(a_1\bar{a}_2 - \bar{a}_1a_2) = \frac{i}{2}[(x_1+iy_1)(x_2-iy_2) - (x_1-iy_1)(x_2+iy_2)] \\ = \frac{i}{2}[(x_1x_2 - iy_2x_1 + iy_1x_2 + y_1y_2) - (x_1x_2 + iy_2x_1 - iy_1x_2 + y_1y_2)] \end{align}$$

Cancel and combine terms: 

$$\begin{align} = \frac{i}{2}[(- iy_2x_1 + iy_1x_2) - (iy_2x_1 - iy_1x_2)] \\ = \frac{i}{2}[-2iy_2x_1 + 2iy_1x_2] = \frac{i}{2}(-2i)(y_2x_1-y_1x_2)\end{align}$$

Some clean up: the 2's cancel and $i (-i) = 1$. So:

$$\begin{align} \frac{i}{2}(-2i)(y_2x_1-y_1x_2) = (x_1y_2 - y_1x_2)\end{align}$$

Plugging back in:
$$\begin{align} \vec{a_1} \times \vec{a_2} \cdot \hat{z} = \frac{i}{2}(a_1\bar{a}_2 - \bar{a}_1a_2) \\ (x_1y_2 - y_1x_2) = (x_1y_2 - y_1x_2)\end{align}$$

The proof is complete.

Problem 2

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