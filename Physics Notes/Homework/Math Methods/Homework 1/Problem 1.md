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