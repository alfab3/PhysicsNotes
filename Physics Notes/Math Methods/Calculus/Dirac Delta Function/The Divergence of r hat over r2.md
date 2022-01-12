A common way to show that $$\nabla \cdot \left(\frac{\hat r}{r^2}\right) = 4\pi\delta(\vec r)$$ is to regularize the function $\left(\frac{\hat r}{r^2}\right)$ in terms of a parameter, say $a$. To that end let $\vec \psi$ be the regularized function given by:

$$\begin{gather} \vec \psi = \frac{\vec r}{(r^2+a^2)^{3/2}}\end{gather}$$ Taking the divergence of this gives: 

$$\begin{gather} \nabla\cdot \vec \psi = \frac{3a^2}{(r^2+a^2)^{5/2}}\end{gather}$$

Now for any sufficiently smooth test function $\phi$ we have that: 

$$\begin{gather} \lim_{a\to 0} \int_V \nabla\cdot \vec \psi\phi(\vec r)\ dV = \lim_{a\to 0} \int_V \frac{3a^2}{(r^2+a^2)^{5/2}} \phi(\vec r) dV = 0\end{gather}$$

If $V$ does not include the origin. 

Now suppose that $V$ does include the origin, Then we have $$\begin{gather} \lim_{a\to 0} \int_V \nabla\cdot \vec \psi\phi(\vec r)\ dV = \lim_{a\to 0} \int_{V-V_\delta} \frac{3a^2}{(r^2+a^2)^{5/2}} \phi(\vec r) dV  + \lim_{a\to 0} \int_{V_\delta} \frac{3a^2}{(r^2+a^2)^{5/2}} \phi(\vec r) dV  \\ = \lim_{a\to 0} \int_{V_\delta} \frac{3a^2}{(r^2+a^2)^{5/2}} \phi(\vec r) dV \end{gather}$$

where $V_\delta$ is a spherical region centered at $\vec r = 0$ with radius $\delta$. For any $\epsilon > 0$, take $\delta > 0$ such that $|\phi(\vec r) - \phi(0)| \leq \epsilon/(4\pi)$ whenever $0<|\vec r| < \delta$. Then we have: 

$$\begin{gather} \lim_{a\to 0}\left|\int_V \nabla\cdot \vec \psi (\phi(\vec r)-\phi(0))dV\right| \leq \lim_{a\to 0} \int_{V_\delta}|\phi(\vec r) - \phi(0)|\frac{3a^2}{(r^2+a^2)^{5/2}}dV \\ \leq  \left(\frac{\epsilon}{4\pi}4\pi\right)\lim_{a\to0}\int^\infty_0 \frac{3a^2}{(r^2+a^2)^{5/2}}r^2dr \leq \epsilon\end{gather}$$

Thus for any test function $\phi$:

$$\begin{gather} \lim_{ a\to 0 } \int_V \nabla \cdot \vec \psi \phi(\vec r) = 4\pi\phi(0)\end{gather}$$ and it is in this sense that:

$$\begin{gather} \lim_{a\to 0} \nabla \cdot \vec \psi = 4\pi\delta(\vec r)\end{gather}$$