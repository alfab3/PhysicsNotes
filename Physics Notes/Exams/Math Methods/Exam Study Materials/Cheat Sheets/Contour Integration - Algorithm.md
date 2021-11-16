## 1.6) Contour Integration (Residue Calculus)
Given an analytic function, the process of evaluating an integral by use of a path in the complex plane.

### 1.6.1)Method of Evaluation 
#### 1.6.1.1) Define the contour

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

#### 1.6.1.2) Rewrite integral
The contour integral now separates into integrals for each segment:

>$$\begin{align}\oint_C = \int_1+\int_2+\ ...\ +\int_n \end{align}$$

#### 1.6.1.3) Evaluate
Residue Theorem
Jordan's Lemma