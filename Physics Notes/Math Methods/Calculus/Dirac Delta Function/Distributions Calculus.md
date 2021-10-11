[[Dirac Delta Function]] and its derivaitves are often called "distribution" or generalized function.

We need to know how they operate on functions in [[Hilbert Space]] $L_2[a,b]$

For example we can start with the [[Heaviside Function]] 

In contrast to $\delta(x)$, $\Theta(x)$ may be thought as an actual function on the Hilbert space $L_2[a,b]$

$$\begin{align}||\Theta(x)|| = \int^b_a|\Theta(x)|^2dx = \int^b_x dx = b - x \end{align}$$

Obviously $\Theta(x)$ is integrable but is discontinous at $x = 0$, so we can define $\delta(x)$ as its [[Derivative]]. Note that for any $f(x) \in L[a,b]$ 

$$\begin{align} \int^b_a\Theta(y-x)f(y)dy = \int^b_af(y)dy = const + F(x) \end{align}$$

The output of the Heaviside acting on $f(x) \in L_2[a,b]$ is the integral $F(x)$.

Now $\int^b_a\delta(x-y)f(y)dy = f(x)$ and we see that the operator $\delta(y-x)$ can act onlt on continuous functions, such that 
$$\begin{align} \lim_{x'\to x^-}f(x') = \lim_{x'\to x^+} f(x') \end{align}$$ and f(x) has a well-defined value that is obtained by the [[Integral]] operation.

Let us consider now: $\frac{d}{dx} \delta(x)$

$$\begin{align} \int^b_a \left[\frac{d}{dx}\delta(x-y)\right] = - \delta(x-y)f(y)\Bigg|^b_{y=a}+\int^b_af'(y)\delta(x-y)=f'(x)\end{align}$$

Hence:
$$\begin{align} \delta'(x-y)\{f(y)\}=f'(x) \end{align}$$

That is the operator $\delta'(x)$ has only meaningful action on the subset of differentiable functions in $L_2[a,b]$