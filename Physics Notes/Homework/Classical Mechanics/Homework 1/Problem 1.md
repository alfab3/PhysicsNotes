Derive: 
$$
m_i\ddot{\vec{r}}_i' = \sum^N_{j=1}-\frac{\partial}{\partial r'_i}U_{ij}(|r'_i-r'_j|)
$$
Using: 
$$
\begin{align} 
	m\ddot{\vec{r}}_i = \sum^N_{j=1} \vec{F}_{ij}\\
	\vec{F}_{ij}=-\frac{\partial}{\partial \vec{r}_i} U_{ij}(\vec{r}_i,\vec{r}_j)
	\\
	U_{ij}(\vec{r}_i,\vec{r}_j) = U_{ji}(\vec{r}_i,\vec{r}_j) \equiv U_{ij}(r_{ij})
	\\r_{ij} = |\vec{r_{i}} - \vec{r_{j}}|
	\\ \vec{r}_i' = \vec{r}_i - v_0t
\end{align}
$$
Start with the left hand side
$$\begin{align} \frac{d^2}{dt^2}[\vec{r}'_i = \vec{r}_i-\vec{v}_0t] \\
\frac{d}{dt}[\dot{\vec{r}}'_i = \dot{\vec{r}}_i-v_o] \\ \ddot{\vec{r}}'_i = \ddot{\vec{r}}_i\end{align}$$

Then the right hand side:
$$\begin{align} |\vec{r}_i' + v_0t - (\vec{r}_j' + v_0t)| \\ |\vec{r}_i' - \vec{r}_j'|\end{align}$$

Prove that the derivative with respect to position will not change:
With chain rule we have 
$$\begin{align} \frac{\partial}{\partial \vec{r}_i'} = \frac{\partial \vec{r_i}}{\partial \vec{r}_i'}\frac{\partial}{\partial \vec{r_i}}\end{align}$$

To prove the relation $\frac{\partial \vec{r_i}}{\partial \vec{r}'_i}$ must equal 1:

$$\begin{align} \frac{\partial \vec{r_i}}{\partial \vec{r_i}'} = \frac{\partial}{\partial \vec{r}_i'}(\vec{r}_i'+v_0t) = \frac{\partial}{\partial \vec{r}_i'}(\vec{r}_i')+\frac{\partial}{\partial\vec{r_i}'}(v_0t) = 1 + 0 = 1\end{align}$$

Therefore:
$$\begin{align} \frac{\partial}{\partial \vec{r_i}'} = \frac{\partial}{\partial \vec{r_i}}\end{align}$$

Now plugging in:
$$
m_i\ddot{\vec{r}}_i' = \sum^N_{j=1}-\frac{\partial}{\partial \vec{r}'_i}U_{ij}(|\vec{r}'_i-\vec{r}'_j|)
$$