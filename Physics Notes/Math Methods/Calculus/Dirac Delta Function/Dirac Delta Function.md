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


Explanation from Math Methods Class
Analogue of the [[Identity operator]] to $\infty$ - dim space

$$\begin{align} I\{f(x)\} = \int^b_a\delta(x-y)f(y)dy = f(x)\end{align}$$