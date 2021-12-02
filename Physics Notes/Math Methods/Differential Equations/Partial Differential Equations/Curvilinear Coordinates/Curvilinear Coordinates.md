### Recap of Cartesian Coordinates

In [[Cartesian Coordinates]] we describe each point $\vec x$ in $3D$ space by a triad $(x,y,z)$ the corresponding unit vectors are defined through the variation of $\vec x (\vec x \rightarrow \vec x + d\vec x)$ upon changing each of the coordinates:

$$\begin{gather} \hat x = \frac{\partial \vec x}{\partial x}; & \hat y = \frac{\partial \vec x}{\partial y}; & \hat z = \frac{\partial \vec x}{\partial z} \end{gather}$$

The triad $(\hat x,\hat y, \hat z) = (\hat i, \hat j, \hat k)$ is everywhere:

Orthogonal:
$$\begin{gather}\hat x \cdot \hat y = \hat z \cdot \hat x = \hat y \cdot \hat z = 0 \end{gather}$$

Fixed in space:
$$\begin{gather} \frac{\partial \hat x}{\partial x} = \frac{\partial \hat x}{\partial y} =\frac{\partial \hat x}{\partial z} = 0 \end{gather}$$

### Orthogonal Curvilinear coordinates 
Describe each point $\vec x$ in space by a triad $(x_1,x_2,x_3)$ 

The corresponding unit vectors are defined similarly: 

$$\begin{gather} \hat e_i =\frac{\partial \vec x}{\partial x_i}/\left|\frac{\partial \vec x}{\partial x_i}\right|\end{gather}$$

The triad $\hat e_1, \hat e_2, \hat e_3$ is everywhere

Orthogonal $$\begin{gather}\hat e_i \cdot \hat e_j = \delta _{ij}\end{gather}$$

Non-fixed in space: namely there exists (at least one) pair $i,j$ such that $$\begin{gather}\frac{\partial \vec x_i}{\partial x_j} \neq  0 \end{gather}$$

### 