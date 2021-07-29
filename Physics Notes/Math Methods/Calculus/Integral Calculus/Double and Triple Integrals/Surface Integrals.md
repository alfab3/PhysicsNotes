Let $dA$ be an element of surface area which projects onto $dxdy$ in the $(x,y)$ planr and let $\gamma$ be the acute angle between $dA$ and the $x,y$ plane. Then we have $$\begin{align} dxdy = dA\cos\gamma \;\; \text{or} \;\; dA=sec\gamma dxdy\end{align}$$ 

The Surface Area is then $$\begin{align} \int\int dA = \int\int \sec\gamma dxdy \end{align}$$

Now we must find $\sec\gamma$. The acute angle between two planes is the same as the acute angle between the normals to the planes. If $\hat{n}$ is a unit vector normal to the surface at $dA$, then $\gamma$ is the acute angle between $\hat{n}$ and the z axis, that is, between the vectors $\hat{n}$ and $\hat{k}$, so $\cos\gamma - |\hat{n} \cdot \hat{k}$|. Let the equation of the surface be $\phi(x,y,z)=$ const. The vector: $$\begin{align} \text{grad} \; \phi = \hat{i}\frac{\partial \phi}{\partial z} + \hat{j}\frac{\partial \phi}{\partial y} + \hat{k} \frac{\partial \phi}{\partial z} \end{align}$$ is normal to the surface  $\phi(x,y,z)=$ const. Then $\hat{n}$ is a unit vector in the direction of grad $\phi$ so $$\begin{align} \hat{n} = (\text{grad}\;\phi)/|\text{grad} \phi |\end{align}$$
This allows us to find that: 
$$\begin{align}\hat{n} \cdot \hat{k} = \frac{\hat{k} \cdot \text{grad}\; \phi}{|\text{grad}\;\phi|} \\ \sec\gamma = \frac{1}{cos\gamma} = \frac{1}{|\hat{n}\cdot\hat{k}|}\end{align}$$
This leads to:
$$\begin{align} \sec\gamma = \frac{|\text{grad} \; \phi|}{|\partial \phi/\partial z|} = \frac{\sqrt{\left(\frac{\partial \phi}{\partial x}\right)^2+\left(\frac{\partial \phi}{\partial y}\right)^2+\left(\frac{\partial \phi}{\partial z}\right)^2}}{|\partial \phi/\partial z|}\end{align}$$

Often the equation of a surface is given in the form $z=f(x,y)$. In this case $\phi(x,y,z) = z -f(x,y)$ , so $\partial \phi \partial z=1$ and this simplifies to $\sec\gamma = \sqrt{(\partial f/\partial x)^2+(\partial f/\partial y)^2 + 1}$. You then substitute $\sec\gamma$ into the integral.