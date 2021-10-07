Frequently we are faced with the problem of describing a quantity that is zero everywhere except a single point, while at that point it is infinite in such a way that its integral over any interval containing that point has a finite value. For this purpose it is useful to introduce the Dirac Delta function, which is defined to have the properties
$$\begin{align} \delta(x) = 0 \; \; \; x \neq 0 \\ f(0) = \int^b_a f(x)\delta(x) dx \end{align}$$

Where $f(x)$ is any well-behaved function and the integration includes the origin. As a special case of the above equation

$$\begin{align} \int^\infty_{-\infty} \delta(x)dx = 1 \end{align}$$
From the definition equation $\delta(x)$ must be an infitely high, thin spike at $x = 0$ as in the description of an impulsive force or the [[Charge Density]] for a [[point charge]]. The problem is that no such function exists, in the usual sense of function. However, the crucial property in the initial equation can be developed rigoursly as the limit of a sequence of functions, a distribution. For example the delta function may be approximated by any of the sequences of functions of the following:
$$\begin{align} \delta_n(x) = \begin{cases} 0, & x < -\frac{1}{2n} \\ n, & -\frac{1}{2n} < x < \frac{1}{2n} \\ 0, & x > \frac{1}{2n} \end{cases} \end{align}$$

$$\begin{align} \delta_n(x) = \frac{n}{\sqrt{\pi}}exp(-n^2x^2) \end{align}$$![[diracfunction.png]]

![[diracfunction2.png]]
$$\begin{align} \delta_n(x) = \frac{n}{\pi} \frac{1}{1+n^2x^2} \end{align}$$
$$\begin{align} \delta_n(x) = \frac{\sin nx}{\pi x} = \frac{1}{2\pi}\int^n_{-n} e^{ixt} dt \end{align}$$

While all these sequences  (and others) cause $\delta(x)$ to have the same properties, they differ somewhat in ease of use for various purposes. The second equation aboce is particulary useful in fourier analysis and in applications to quantum mechanics. In the theory of Fourier Series this often appears as the Dirchlet kernel
$$\begin{align} \delta_n(x) = \frac{1}{2\pi} \frac{sin[(n+1\frac{1}{2})x]}{sin(\frac{1}{2}x)}\end{align}$$

The forms for $\delta_n(x)$ given in the equations above all obviously peak strongly for large $n$ at $x = 0$. 

Properties of $\delta(x)$
1) Dirac's delta function must be even in $x$, $\delta(-x) = \delta(x)$
2) If $a>0$ $$\begin{align}\delta(ax) = \frac{1}{a}\delta(x), \; \; a > 0 \end{align}$$ which can be proved by making the substitution $x = y/a$ $$\begin{align} \int^\infty_{-\infty} f(x)\delta(ax)dx = \frac{1}{a} \int^\infty_{-\infty} f(y/a) \delta(y)dy = \frac{1}{a}f(0) \end{align}$$ If $a < 0$ the main equation becomes $\delta(ax) = \delta (x)/|a|$
3) Shift of origin $$\begin{align} \int^\infty_{-\infty} \delta(x-x_0)f(x)dx = f(x_0) \end{align}$$ which can be proved by making the substitution $y = x - x_0$ and noting that when $y = 0$, $x = x_0$.
4) If the argument of $\delta(x)$ is a function $g(x)$ with simple zeros at points $a_i$ on the real axis $$\begin{align} \delta \bigg((g(x))\bigg) = \sum_i\frac{\delta(x-a_i)}{|g'(a_i)|} \end{align}$$ To prove this equation we write $$\begin{align} \int^\infty_{-\infty} f(x) \delta(x) dx = \sum_i \int^{a_i + \epsilon}_{a_i-\epsilon} f(x) \delta ((x-a_i)g'(a_i))dx \end{align}$$ where we have decomposed the original integral into a sum of integrals over small intervals containing the zeros of $g(x)$ by the leading term in its Taylor series.
5) Derivative of delta function: $$\begin{align} \int^\infty_{-\infty} f(x) \delta'(x-x_0)dx = -\int^\infty_{-\infty} f'(x)\delta(x-x_0)dx = -f'(x_0)\end{align}$$ Defining the dericative $\delta'(x)$; it is evaluated by performing integration by parts on any of the sequences defining the delta function.
6) In three dimensions the delta function $\delta(\vec{r})$ is interpreted as $\delta(x)\delta(y)\delta(z)$, so it describes a function localized at the origin and with unit integrated weight, irrespective of the coordinate system in use. Thus, in spherical polar coordinates$$\begin{align} \int \int \int f(\vec{r_2}) \delta(\vec{r_2}-\vec{r_1})r^2_2dr_2\sin \theta_2d\theta_2d\phi_2 = f(\vec{r_1}) \end{align}$$
7) $$\begin{align} \delta(t-x) = \frac{1}{2\pi}\int^\infty_{-\infty} exp(i\omega(t-x))d\omega \end{align}$$ with the understanding that this has meaning only when under an integral sign in that context it is extremely useful for the simplification of fourier integrals
8) Expansions of $\delta(x)$