You find maximum and minimum points of $y(x)$ by setting $dy/dx = 0$ For a surface represented by the function $z=f(x,y)$. If there is a maximum point on it then the curves for $x = \text{const}$ and $y = \text{const}$ which pass through the maximum point also have a maxima at the same point. That is, $\partial z / \partial x$ and $\partial z / \partial y$ are zero at the maximum point.  The point where  $\partial z / \partial x = 0$ and  $\partial z / \partial y = 0$ might be a maximum, minimum, or neither (saddle point). To determine if the point is a max or min you must perform the operation $\partial^2 y / \partial x^2$

Example:
A pup tent of given volume $V$, with ends but no floor is to be made using the least possible material. Find the proportions

The bottom has dimensions of $l$ and $2w$ with the angles of the triangle on the side of length $2w$ are both $\theta$

Using the letters indicated above we find the volume $V$ and the area $A$ 
$$\begin{align} V = \frac{1}{2} \cdot 2w \cdot w \tan \theta = w^2l\tan\theta \\ A = 2w^2 \tan\theta + \frac{2lw}{\cos\theta}\end{align}$$

Since V is given only two of the three variables $w, l, \text{and} \; \theta$ are independent and we must eliminate one of them from $A$ before we try to minimize $A$. Solving the $V$ equation for $l$ and substituting into $A$ we get $$\begin{align}A = 2w^2\tan\theta + \frac{2w}{\cos\theta}\frac{V}{w^2\tan\theta} = 2w^2\tan\theta+\frac{2V}{w}\csc\theta\end{align}$$

We now have $A$ as a function of two independent variables $w$ and $\theta$. To minimize $A$ we find $\partial A/\partial w$ and $\partial A/\partial \theta$ and set them equal to zero.
$$\begin{align}\frac{\partial A}{\partial w} = 4w\tan\theta-\frac{2V \csc \theta}{w^2} = 0\\ \frac{\partial A}{\partial \theta} = 2w^2\sec^2\theta-\frac{2V}{w}\csc\theta\cot\theta = 0\end{align}$$

Solving each of these equations for $w^3$ and setting the results equal we get $$\begin{align} w^3 = \frac{V\csc\theta}{2\tan\theta} = \frac{V\csc\theta\cot\theta}{\sec^2\theta}\;\;\; \text{or}\;\;\; \frac{\cos\theta}{2sin^2\theta} = \frac{\cos\theta \cos^2\theta}{sin^2\theta}\end{align}$$
