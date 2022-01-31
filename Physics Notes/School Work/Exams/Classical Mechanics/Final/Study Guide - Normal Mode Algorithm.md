## Process
1) Determine the Bilinearized Lagrangian
2) Establish $\mathcal M$ (mass) matrix: $$\begin{gather} \frac{\partial \mathcal L}{\partial \dot{\vec x}} = \mathcal M\dot{\vec x} \end{gather}$$
3) Establish $\mathcal K$ (potential) matrix: $$\begin{gather} \frac{\partial \mathcal L}{\partial \vec x} = - \mathcal K\vec x \end{gather}$$
4) Write characteristic equation: $$\begin{gather} \det(\mathcal K - \lambda \mathcal M) = 0\end{gather}$$
5) Solve determinant and determine eigenvalues (if possible)
6) Solve for Eigenvectors: $$\begin{gather} (\mathcal K - \lambda_s \mathcal M)\vec u_s = 0, & \vec u_s \equiv (u_{s1},u_{s2}), & (s=1,2) \end{gather}$$
7) This is just a matter of normalization, we can easily set $u_{s1} = 1$ and solve for $u_{s2}$
8) Make small angle approximations
	1) General Rules: $$\begin{gather} \sin\theta \approx \theta \\ \cos\theta \approx 1 - \frac{\theta^2}{2} \\ \tan\theta \approx \theta  \\ e^x \approx 1 + x \end{gather}$$
	2) For a rule like: $m_1 \ll m_2$: $$\begin{gather} \left(1+\frac{m_1}{m_2}\right) \approx1\end{gather}$$

Examples: 

[[Problem 28]]
[[Problem 29]]