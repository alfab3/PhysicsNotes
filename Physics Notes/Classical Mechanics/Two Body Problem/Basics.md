Consider the problem of two interacting particles:
$$
m_1\ddot{r}_1 = F_{12}
$$
$$
m_2\ddot{r}_2 = F_{21}
$$

We already know that the center of mass
$$
\vec{R} = \frac{m_1 \vec{r}_1 + m_2\vec{r}_2}{m_1 + m_2}
$$
moves with a constant velocity:
$$
\vec{R}(t)=\vec{V_0}t
$$

$$
\vec{V_0} = \frac{m_1 \vec{v}_1^{(0)}+m_2\vec{v}_2^{(0)}}{m_1+m_2}
$$
where $\vec{v}_1^{(0)}$ and $\vec{v}_2^{(0)}$ are the initial velocities of the particles;  without loss of generality we choose $\vec{R}(t=0)=0$. 

Another natural and convenient variable is the vector of relative distance:
$$
\vec{r}=\vec{r}_1-\vec{r}_2
$$

Given $r$ and $R$, one immediately finds $\vec{r}_1$ and $\vec{r}_2$:
$$
\vec{r}_1 = \vec{R}+\frac{m_2}{m_1+m_2}\vec{r}
$$
$$
\vec{r}_2 = \vec{R} - \frac{m_1}{m_1 + m_2}\vec{r}
$$
We want to set up a problem for finding $\vec{r}$. To this end we multiply the initial equations by $m_1$, then subtract one from another. As a result, we get
$$
m_*\ddot{r}=\vec{F}(\vec{r})
$$
$$
m_* = \frac{m_1m_2}{m_1+m_2}
$$
$$
\vec{F}(\vec{r}) = -\frac{\partial U_{12}(r)}{\partial \vec{r}} = -\frac{\vec{r}}{r} \frac{dU_{12}{r}}{dr}
$$