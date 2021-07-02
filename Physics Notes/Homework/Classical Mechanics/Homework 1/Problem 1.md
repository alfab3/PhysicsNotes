Derive: 
$$
m_i\ddot{r} = \sum^N_{j=1}-\frac{\partial}{\partial r'_i}U_{ij}(|r'_i-r'_j|)
$$
Using: 
$$
\begin{align} 
	m\ddot{\vec{r}}_i = \sum^N_{j=1} \vec{F}_{ij}\\
	\vec{F}_{ij}=-\frac{\partial}{\partial \vec{r}_i} U_{ij}(\vec{r}_i,\vec{r}_j)
	\\
	U_{ij}(\vec{r}_i,\vec{r}_j) = U_{ji}(\vec{r}_i,\vec{r}_j) \equiv U_{ij}(r_{ij})
	\\r_{ij} = |\vec{r_{i}} - \vec{r_{j}}|
\end{align}
$$
Start with the left hand side
$$\begin{align} \frac{d^2}{dt^2}[\vec{r}'_i = \vec{r}_i-\vec{v}_0t] \\
\frac{d}{dt}[\dot{\vec{r}}'_i = \dot{\vec{r}}_i-v_o] \\ \ddot{\vec{r}}'_i = \ddot{\vec{r}}_i\end{align}$$
Then the right hand side:
$$\begin{align} |\vec{r}_i' + v_0t - (\vec{r}_j' + v_0t)| \\ |\vec{r}_i' - \vec{r}_j'|\end{align}$$

Gives us:
$$
m_i\ddot{r} = \sum^N_{j=1}-\frac{\partial}{\partial r'_i}U_{ij}(|r'_i-r'_j|)
$$