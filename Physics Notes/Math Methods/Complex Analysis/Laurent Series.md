Assume $f(z)$ is an [[Analytic Function]] in a punctuated domain $(\Omega/z_0)$

Then $$\begin{align} f(z) = \sum^\infty_{n=-\infty} a_n (z-z_0)^n \end{align}$$

Where: $$\begin{align} a_n = \frac{1}{2\pi i}\oint_\Gamma\frac{f(z')}{(z'-z_0)^{n+1}} \end{align}$$

For a non-essential [[Singularity]], we can compute the reside easily:

$$\begin{align} g(z) = (z-z_0)^m f(z) = (z-z_0)^m\sum^\infty_{n=-m} a_m(z-z_0)^n = \\\sum^\infty_{n=0} a_{n-m}(z-z_0)^n \end{align}$$

Hence: 
$$\begin{align} a_{n-m} = \frac{1}{n!}g^n(z_0) = a_n=\frac{1}{(n+m)!}g^{(n+m)}(z_0)\\ Res[f,z_0] = a_{-1}=\frac{1}{(m-1)!}g^{(m-1)}(z_0)\end{align}$$

