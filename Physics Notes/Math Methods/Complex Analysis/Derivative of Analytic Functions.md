The derivative of $f(z)$ at some point z in the complex plane. $z\rightarrow z+ \delta z$. 
$$\begin{equation}
    \frac{df}{dz} = \lim_{dz\to\infty} \frac{f(z+\delta z - f(z)}{\delta z}
\end{equation}$$
In which direction though? To solve for that we need the general case:
$$\begin{equation}
    \delta z = \epsilon e^{i\alpha}
\end{equation}$$
Combining them:
$$\begin{equation}
    \frac{df}{dz} = e^{-i\alpha}((\frac{\partial u}{\partial x}cos\alpha + i\frac{\partial v}{\partial y}sin\alpha) - i(\frac{\partial u}{\partial y} cos \alpha - i\frac{\partial v}{\partial x}sin\alpha))
\end{equation}$$
What direction should $\alpha$ be? The direction shouldn't matter regardless of the direction that $\delta z$ goes to zero. No matter how you approach to zero you will have the same answer, there is no uniqueness in the derivative. Can this be independent of $\alpha$? The only condition where it is independent of $\alpha$ if if the Cauchy-Riemann conditions are satisfied.\\

In the case of complex of variables, if a function is analytic at a certain point it means its got a derivative, this derivative itself is an analytic function. Therefore it has a derivative that is an analytic function, and so on. So every analytic function is infinitely differentiable at any given point. If $f(z)$ is analytic all its derivatives are also analytic. What this implies is that you have a very useful representation for analytic functions in some reason its analytic. If a function is analytic in some region R, if you have some point in the region $z_0$ you can represent $f(z)$ as a power series 
$$\begin{equation}
    f(z) = \sum_{n=0}^{\infty} a_n(z-z_0)^n
\end{equation}$$
Which is a Taylor series
$$\begin{equation}
    a_n = \frac{1}{n!}\frac{d^n}{dz^n} f(z) \; z=z_0
\end{equation}$$
Where would this series converge? Such a series has a region of convergence, called its circle of absolute convergence. So you have some point $z$ you have some circle around it with radius R inside which $\sum_{n=0}^\infty |a_n(z-z_0)^n| < \infty$ converges absolutely. Where the radius (also called the radius of convergence) is found by:
$$\begin{equation}
    R = \lim_{n\to\infty} |\frac{a_n}{a_{n+1}}|
\end{equation}$$
Ratio test is this ratio is less than 1 then you have convergence if not then you don't. This limit may not exist in some cases. We need a more general case.
$$\begin{equation}
    R = \lim_{n\to\infty} sup |a_n|^{1/n}
\end{equation}$$