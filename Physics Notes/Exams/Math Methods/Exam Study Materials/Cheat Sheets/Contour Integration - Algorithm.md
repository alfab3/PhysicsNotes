## Contour Integration (Residue Calculus)
Given an analytic function, the process of evaluating an integral by use of a path in the complex plane.

### Method of Evaluation 

#### Find Poles
Determine where the integrand is undefined
#### Define the contour

##### Rational Function 
>$$\begin{align} \int^\infty_{-\infty} F(x)dx \end{align}$$

where $F(x)$ is a rational function. 
Consider $\oint_C F(z)dz$ along a contour $C$ consisting of the line along the $x$ axis from $-R$ to $+R$ and the semicircle $\Gamma$ above the x axis having this line as diameter. Then, let $R \to \infty$. If $F(x)$ is an even function, this can be used to evaluate $\int^\infty_0 F(x)dx$

##### Rational Function with sine or cosine
>$$\begin{align}\int^{2\pi}_0 G(\sin \theta, \cos \theta)d\theta \end{align}$$

Where $G(\sin\theta, \cos\theta)$ is a rational function of $\sin \theta$ and $\cos \theta$

Let $z = e^{i\theta}$. Then $\sin \theta = (z -z^{-1})/2$, $\cos \theta = (z + z^{-1})/2$ and $dz = ie^{i\theta} d\theta$ or $d\theta = dz/iz$. The given integral is equivalent to $\oint_C F(z)dz$ where $C$ is the unit circle with center at the origin.


##### Sector Contour $(0, \infty)$
An integral on the real range $(0,\infty)$ that lacks the symmetry needed to extend the integration range to $(-\infty,\infty)$

Consider: 
>$$\begin{align} I = \int^\infty_0 \frac{dx}{x^3+1}  \end{align}$$

Solve for the pole:
>$$\begin{gather} x^3+1=0 \\ x^3 = -1 \\  x^3 =e^{i\pi} \\ x = e^{i\pi/3}\end{gather}$$

So now we can set the sector contour to include this pole, we choose the angle: $\theta = 2\pi/3$

##### Rectangular contour
Solve for poles, if when you take $R \to \infty$ a semicircle will enclose infinitely many poles, you must use a rectangular contour.

##### A pole on the Contour

Example: 
>$$\begin{align} I = \int^{\infty}_{-\infty} \frac{\cos x}{x}dx\end{align}$$

Use a semicircle that avoids the singularity (Annulus)

##### Branch Cuts

We can construct a contour around the discontinuity to solve the integral. Example:
>$$\begin{align} J = \int_C \frac{\ln z dz}{z^3 +1}\end{align}$$

####  Rewrite integral
The contour integral now separates into integrals for each segment:

>$$\begin{align}\oint_C = \int_1+\int_2+\ ...\ +\int_n \end{align}$$

####  Evaluate
Residue Theorem
Jordan's Lemma

##  Principal Value Theorem

The Cauchy Principle Value of an integral of the form:

>$$\begin{gather} \int^\infty_{-\infty}\frac{f(x)}{x-x_0}dx  \end{gather}$$

is given by
>$$\begin{gather} P\int^\infty_{-\infty} \frac{f(x)}{x-x_0}dx = 2\pi i \sum_{z_j} \frac{1}{z_j-x_0} \text{Res}[f(z),z_j] + \pi i f(0) \end{gather}$$

where $z_j$ is the set of all residues of $f(z)$ in the upper half complex plane. This is a way to assign values to integrals that would otherwise be divergent from the perspective on the real line. An alternative but equivalent definition of the principal value for the same form of the integral is given by:

>$$\begin{gather} P\int^\infty_{-\infty} \frac{f(x)}{x-x_0}dx = \lim_{\delta\to 0} \frac{(x-x_0)f(x)}{(x-x_0)^2+\delta^2} dx\end{gather}$$

More generally, the principle value of an integral of the form 
>$$\begin{gather} \int^b_a g(x)dx \end{gather}$$

where $g(x)$ has $n$ singularities $x_1 < x_2 < x_3 < ... < x_n$ is defined as:

>$$\begin{gather} P\int^b_a g(x)dx = \\\lim_{\delta_i \to 0}\left[\int^{x_0 - \delta_0}_a g(x)dx + \int^{x_1 - \delta_1}_{x_0 - \delta_0} g(x)dx + \int^{x_2 - \delta_2}_{x_1 - \delta_1} g(x)dx + ...+\int^{b}_{x_0 - \delta_0} g(x)dx\right] \end{gather}$$

Example 1)

Consider the following integral: 

$$\begin{gather} \int^\infty_{-\infty} \frac{1}{x(x^3-1)} \end{gather}$$

$\underline{\text{Method 1}}$

Step 1: Find the poles

$$\begin{gather} x(x^3+1) = 0 \\ x = 0,\; x = -1, \;x = e^{i\pi/3}\end{gather}$$

Step 2: Define the Contour
![[pv contour 1.png]]

Where the contour is a semi-circle, with holes cut out at both points on real axis of radius $\delta$ and $\epsilon$

Step 3: Construct the Integral

$$\begin{gather} P\int^\infty_{-\infty} \frac{dx}{x(x^3+1)} = \oint_\Gamma \frac{dz}{z(z^3+1)} = \\ \int^{-1-\delta}_{-R}\frac{dx}{x(x^3+1)} + \int^{0}_{\pi}\frac{i\delta e^{i\theta} d\theta}{(-1+\delta e^{i\theta})[({-1+\delta e^{i\theta})^3}+1]} + \int_{-1+\delta}^\epsilon\frac{dx}{x(x^3+1)} \\ + \int^{0}_{\pi}\frac{i\epsilon e^{i\theta} d\theta}{\epsilon e^{i\theta}({\epsilon e^{3i\theta}}+1)} + \int_{\epsilon}^{R}\frac{dx}{x(x^3+1)} +\int^{\pi}_{0}\frac{iR e^{i\theta} d\theta}{R e^{i\theta}({R e^{3i\theta}}+1)} \end{gather}$$

Step 4: Evaluate Angular Integrals

Let us begin with the semi-circle of radius $R$
>$$\begin{gather} \lim_{R \to \infty}\int^{\pi}_{0}\frac{iR e^{i\theta} d\theta}{R e^{i\theta}({R e^{3i\theta}}+1)} \to 0\end{gather}$$Jordan's Lemma

Now for the semi-circle of radius $\delta$

>$$\begin{gather} \lim_{\delta \to\infty}\int^{0}_{\pi}\frac{i\delta e^{i\theta} d\theta}{(-1+\delta e^{i\theta})[({-1+\delta e^{i\theta})^3}+1]} \end{gather}$$

I am too lazy to write this out, using L'Hopital's rule we get:

$$\begin{gather}\frac{\pi i}{3} \end{gather}$$

Lastly for the semi-circle of radius $\epsilon$
>$$\begin{gather} \int^{0}_{\pi}\frac{i\epsilon e^{i\theta} d\theta}{\epsilon e^{i\theta}({\epsilon e^{3i\theta}}+1)} = -i\pi f(0) = -i\pi\end{gather}$$

Step 4: Evaluate Integrals along the real line:

>$$\begin{gather} \int^{-1-\delta}_{-R}\frac{dx}{x(x^3+1)} +  \int_{-1+\delta}^\epsilon\frac{dx}{x(x^3+1)} + \int_{\epsilon}^{R}\frac{dx}{x(x^3+1)} = P\int^\infty_{-\infty} \frac{dx}{x(x^3+1)} \\ P\int^\infty_{-\infty} \frac{dx}{x(x^3+1)}  = \frac{2\pi i }{e^{i\pi/3}} \text{Res}\left[\frac{1}{z^3+1},e^{i\pi/3}\right]+i\pi-i\pi/3\\ = 2\pi ie^{-i\pi/3}\lim_{z\to e^{i\pi/3}}\left[\frac{z-e^{i\pi/3}}{z^3+1}\right] + \frac{2i\pi}{3} \\ = -\frac{2i\pi}{3} + \frac{2i\pi}{3} = 0 \end{gather}$$