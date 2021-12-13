## Relation to Differential Operators

Consider $\mathcal L y(\vec x) = f(\vec x)$ with $f(\vec x) \neq 0$ with some [[Boundary Condtion]]. 

Then $\mathcal L$ is "invertible" if it has no zero modes. Namely, no solutions to $\mathcal Ly(\vec x) = 0$ (except the trivial one: $y(\vec x) = 0$) And $\mathcal L$ is non-invertible if it does have zero modes. 

Fredholm alternative (just like for finite dim matrices)

If $\mathcal L$ is invertible then $\mathcal Ly(\vec x) = f(\vec x)$ has a unique solution that can be written formally as $$\begin{gather} y(\vec x) = \mathcal L^{-1}f(\vec x) \end{gather}$$.

If $\mathcal L$ is "non-invertible" then $\mathcal L y(\vec x) = f(\vec x)$ has a solution is  $\braket{f(\vec x)|u(\vec x)} = 0$ ([[Inner Product]]) for all zero-modes of $\mathcal L^\dagger$, i.e. $\vec u(x)$ such that $\mathcal L^\dagger u(\vec x) = 0$

#### Example: 
Consider $\mathcal L = -\frac{d^2}{dx^2}$ where $x \in (0,1)$ with boundary condition $$\begin{gather}\frac{dy}{dx}\bigg|_{x=0} = \frac{dy}{dx}\bigg|_{x=1} = 0\end{gather}$$ consider the equation $$\begin{gather} -\frac{d^2y}{dx^2} = f(x) \end{gather}$$with some $f(x) \neq 0$ Is there a solution to this equation.

Answer: To apply Fredholm alternative we need to consider $\mathcal L^\dagger$ we showed that $\mathcal L^\dagger = \mathcal L$ and $D(\mathcal L^\dagger) = D(\mathcal L)$ (so $\mathcal L$ is self-adjoint)

Now, $\mathcal L^\dagger$ has a zero mode $u(x)=1$

Indeed: $$\begin{gather} -\frac{d^2u}{dx^2}=0  \end{gather}$$ and $$\begin{gather} \frac{du}{dx}\Bigg|_{x=0} = \frac{du}{dx}\Bigg|_{x=1} = 0\end{gather}$$

Hence: 

$$\begin{gather} -\frac{d^2y}{dx^2}=f(x) \end{gather}$$ has a solution only if $$\begin{gather} \braket{f(x)|u(x)} = 0 \end{gather}$$