### Definition 
Let us consider two opposite point charges and assume we are interested in finding $\phi(\vec x)$ at some point since there is obviously an axial symmetry with respect to the axis that connects the two charges, it is useful to choose it as our z-axis, with the origin at the middle point between the two charges such that

$$\begin{gather} \phi(\vec x) = \phi(r,\theta,\phi) = \sum^\infty_{l=0}[A_lr^l+B_lr^{-(l+1)}]P_l(\cos\theta)\end{gather}$$

which is the form of the [[Solution of Laplace Equation]]

![[electric dipole.png]]
we would like to compute the coefficients $A_l$ and $B_l$, Before doing the actual calculation, let us note that we mus distinguish between two limits:

$r \to 0$ or more generally $r \ll d$. Here since $\phi \to \text{const}$ we see that $\{B_l\}=0$

$r \to \infty$ (or more generally $r \gg d$): 
Gere since $\phi \to 0$ we see that $\{A_l\}=0$

This means the solution is not uniform. That is, the unavoidable singularities at $r = \pm d$ (due to the point charges) give rise to two separate expansions in terms of spherical harmonics ("near-field" and "far field")

### Constructing the Potential Form

In order to find $A_l$ and $B_l$, lets us recall basic electrostatics, where we obtain the [[Electric Potential]] through "superposition" of the potential induced by the two point charges:

$$\begin{gather} \phi(\vec x) = \frac{q}{4\pi\epsilon_0}\left[\frac{1}{\sqrt{r^2+d^2-2rd\cos\theta}} - \frac{1}{\sqrt{r^2+d^2+2rd\cos\theta}}\right] \end{gather}$$

Comparing this to the general form of our solution we note that we can get them to a similar form by Taylor-expanding ([[Taylor Series]]) the "square root" function crucially since the coefficients $A_l$, $B_l$ do not depend on $r$ and $\theta$ we can choose any $\theta$ we want to make this comparison.

Let us choose $\theta = 0(\cos\theta = 1)$ Then:

$$\begin{gather} \phi(\vec x) = \frac{q}{4\pi\epsilon_0}\left[\frac{1}{\sqrt{r^2+d^2-2rd}} - \frac{1}{\sqrt{r^2+d^2+2rd}}\right] \end{gather}$$

Let us address first $r \gg d$ ("far-field")

Here: 

$$\begin{gather} \frac{1}{\sqrt{r^2+d^2\pm 2rd}} = \frac{1}{r\sqrt{1+(d/r)^2+2(d/r)}} \end{gather}$$

substituting $y = d/r$ and Taylor expanding at $y=0$ we get:

$$\begin{gather} \phi(r,\theta = 0) = \frac{q}{4\pi\epsilon_0}\left[\frac{d}{r^2}+\frac{d^3}{r^4}+\frac{d^5}{r^6}+ \ldots\right] \end{gather}$$

Comparing with $(x)$ we get: 

$$\begin{gather} \{A_l = 0\} & B_{2n} = 0 & B_{2n+1} = \frac{d^{2n}q}{2\pi\epsilon_0} \end{gather}$$

Now consider the "near-field" $r \ll d$

Here: 

$$\begin{gather}\frac{1}{\sqrt{r^2+d^2\pm 2rd}} = \frac{1}{d\sqrt{1+(r/d)^2+2(r/d)}} \end{gather}$$

substituting $y = r/d$ and Taylor-expanding around $y = 0$ we get: 

$$\begin{gather} \phi(r,\theta = 0) = \frac{q}{4\pi\epsilon_0}\left[\frac{r}{d^2}+\frac{r^3}{d^4}+\frac{r^5}{d^6}+ \ldots\right] \end{gather}$$

Comparing with $(x)$ we get: 

$$\begin{gather} \{B_l=0\} & A_{2n} = 0 & A_{2n-1} = \frac{d^{-2n}q}{2\pi \epsilon_9}\end{gather}$$