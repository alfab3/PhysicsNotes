The $x$, $y$ plane only allows the real variable to tend to either plus or minus $x$, and the same for $y$. 
In the complex plane there is an infinite number of directions that can tend to infinity. Our Riemann sphere: 
On the sphere ($S$) the coordinates are 
$$\begin{align}
    \Psi_1 = sin\theta cos\phi\\
    \Psi_2 = sin\theta sin\phi\\
    \Psi_3 = cos\theta
\end{align}$$
Mapping the complex plane to the surface of the sphere, every point that exists on the complex plane there exists a point on the sphere. All points within the unit circle are mapped from the southern hemisphere. The south pole is mapped to the origin.
From here we can construct:
$$\begin{equation}
    \frac{\Psi_2}{y}=\frac{1-\Psi_3}{1}
\end{equation}$$
Which gives us:
$$\begin{align}
    y = \frac{\Psi_2}{1-\Psi_3}\\
    x = \frac{\Psi_1}{1-\Psi_3}\\
    z = \frac{\Psi_1 + i\Psi_2}{1-\Psi_3}\\
    z* = \frac{\Psi_1 - i\Psi_2}{1 - \Psi_3}
\end{align}$$
Now plugging in 1.3 - 1.5:
$$\begin{align}
    x = (cot\frac{\theta}{2})cos\phi\\
    y = (cot\frac{\theta}{2})sin\phi\\
    z = e^{i\phi}cot\frac{\theta}{2}\\
    z* = e^{-i\phi}cot\frac{\theta}{2}
\end{align}$$
Their respective reverse mappings are given by: 
$$\begin{align}
    \Psi_1 = \frac{2x}{x^2+y^2+1} = \frac{z + z*}{|z|^2 + 1}\\
    \Psi_2 = \frac{2y}{x^2+y^2+1} = \frac{z - z*}{i|z|^2 + 1}\\
    \Psi_2 = \frac{x^2+y^2-1}{x^2+y^2+1} = \frac{|z|^2 - 1}{|z|^2 + 1}
\end{align}$$
How is distance defined on the sphere?
$$\begin{equation}
    |z_1 - z_2|
\end{equation}$$
Distance between two points on the complex plane can be defined by the chordal distance:
$$\begin{equation}
    d(z_1,z_2) = \frac{2|z_1 - z_2|}{\sqrt{(|z_1|^2+1) (|z_2|^2+1)}}
\end{equation}$$

$$\begin{align}
    d(z_1,z_2) = 0 \; iff \; z_1 = z_2\\
    d(z_2, z_1) = d(z_1,z_2) \geq 0\\
    d(z_1, z_3 \leq d(z_1,z_2) + d(z_2,z_3)\\
    d(z, \infty) = \frac{2}{\sqrt{|z|^2+1}}
\end{align}$$