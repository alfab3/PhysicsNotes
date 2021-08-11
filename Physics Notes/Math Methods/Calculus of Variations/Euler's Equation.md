A typical problem arising in connection with a [[Functional]] $F[f]$ is the problem of finding a function $f$ that minimizes or maximizes the functional

Suppose the function $f$ is a local max or min of the functional $F$. Then for any small variation of the function $f$, the variation of the functional has to be sign-definite. Let use see what are the implications of this fact. We introduce the symbol $\delta f(x)$ for an infinitesimal variation of the function $f$ and the symbol $\delta F$ for corresponding variation of the functional $F$. That is
$$
\delta F = F[f+\delta F] - F[f]
$$
With a simple observation that 
$$
f\rightarrow f + \delta f \Rightarrow f_x \rightarrow f_x + (\delta f)'
$$
we have 
$$
\delta F = \int^{x_b}_{x_a} g(f+\delta f, f_x + (\delta f)',x)dx - \int^{x_b}_{x_a} g(f,f_x,x)dx
$$
...
$$
\delta F = \int^{x_b}_{x_a} A(x)\delta f(x)dx
$$
where 
$$
A(x)=\frac{\partial g}{\partial f} - \frac{d}{dx} \frac{\partial g}{\partial f_x}
$$
$$
A(x) \equiv \frac{\delta F}{\delta f(x)}
$$
This allows us to arrive at the equation 
$$
\frac{\partial g}{\partial f} - \frac{d}{dx}\frac{\partial g}{\partial f_x} = 0
$$
Functional of many functions
Now if we are looking for minimum/maximum of the functional F, then by definition we have $\delta F \geq 0$ for a minimum or $\delta F \leq 0$ for a maximum And this is only possible if 
$$
A_j(x) \equiv 0
$$
The Euler equation then becomes:
$$
\frac{\partial g}{\partial f^{(j)}} - \frac{d}{dx}\frac{\partial g}{\partial f_x^{(j)}} = 0
$$

Boas: 

Before we do the general problem let us first do the problem of a geodesic on a plane; we shall show that a straight line gives the shortest distance between two points. Our problem is to find $y=y(x)$ which will make $$\begin{align} I = \int^{x_2}_{x_1} \sqrt{1+y'^2} dx \end{align}$$ as small as possible. The $y(x)$ which does this is called an external. How we want some way to represent algebraically all the curves passing through the given end-points, but differing from the external by small amounts. These curves are called varied curves; there are infinitely many of them as close as we like to the extremal. We construct a function representing these varied curves in the following way. 

![[varied curves.png]]

Let $\eta(x)$ represent a function of $x$ which is zero at $x_1$ and $x_2$, and has a continuous second derivative in the interval $x_1$ to $x_2$, but is otherwise completely arbitrary. We define the function $Y(x)$ by the equation $$\begin{align} Y(x) = y(x) + \epsilon\eta(x) \end{align}$$ where $y(x)$ is the desired extremal and $\epsilon$ is a parameter. Because of the arbitrariness of $\eta(x)$, $Y(x)$ represents any single-valued curve you want to draw through $(x_1,y_2)$ and $(x_2,y_2)$. Out of all these curves $Y(x)$ we want to pick the one curve that makes $$\begin{align} I = \int^{x_2}_{x_1} \sqrt{1+Y'^2}dx \end{align}$$ a minimum. Now $I$ is a function of the parameter $\epsilon$; when $\epsilon = 0$, $Y = y(x)$, the desired extremal. Our problems then is to make $I(\epsilon)$ take its minimum value when $\epsilon = 0$. In other words, we want $$\begin{align} \frac{dI}{d\epsilon}= 0\end{align}$$ when $\epsilon = 0$. Differentiating under the integral sign with respect to the parameter $\epsilon$, we get $$\begin{align}\frac{dI}{d\epsilon} = \int^{x_2}_{x_1}\frac{1}{2} \frac{1}{\sqrt{1+Y'^2}}2Y'\left(\frac{dY'}{d\epsilon}\right)dx \end{align}$$
Differentiating with respect to $x$ we get $$\begin{align} Y'(x) = y'(x)+\epsilon\eta'(x) \end{align}$$

Then:
$$\begin{align} \frac{dY'}{d\epsilon} = \eta'(x) \end{align}$$

We see that putting $\epsilon = 0$ means putting $Y(x) = y(x)$. The substituting and putting $dI/d\epsilon$ equal to 0 when $\epsilon = 0$ we get $$\begin{align} \left(\frac{dI}{d\epsilon}\right)_{\epsilon=0} = \int^{x_2}_{x_1} \frac{y'(x)\eta'(x)}{\sqrt{1+y'^2}}dx = 0 \end{align}$$

We can then integrate this by parts ([[Integration by Parts]]). Let: $u = y'/\sqrt{1+y'^2}$ and $dv = \eta'(x)dx$

Then $du = \frac{d}{dx}\left(\frac{y'}{\sqrt{1+y'^2}}\right)dx$, and $v = \eta(x)$

and 

$$\begin{align} \left(\frac{dI}{d\epsilon}\right)_{\epsilon=0} = \frac{y'}{\sqrt{1+y'^2}}\eta(x)\bigg|^{x_2}_{x_1} - \int^{x_2}_{x_1}\eta(x)\frac{d}{dx}\left(\frac{y'}{\sqrt{1+y'^2}} \right)dx\end{align}$$

The firs term is zero because $\eta(x) = 0$ at the endpoints. In the second term recall that $\eta(x)$ is an arbitrary function. 
$$\begin{align} \frac{d}{dx} \left(\frac{y'}{\sqrt{1+y'^2}}\right)=0\end{align}$$

Integrating this with respect to $x$, we get 
$$\begin{align} \frac{y'}{\sqrt{1+y'^2}} = \text{const.}\end{align}$$

or $y' =$ const. Thus the slope of $y(x)$ is constant, so $y(x)$ is a straight line as we expected. 

We could go through this process with every calculus of variations problem. It is much simpler to do the general problem once for all and find a differential equation which we can use to solve later problems. The problem is to find the $y$ which will make stationary the integral $$\begin{align}I = \int^{x_2}_{x_1} F(x,y,y')dx \end{align}$$
where $F$ is a given function. The $y(x)$ which makes the $I$ stationary is called an extremal whether $I$ is a maximum or minimum or neither. The method is the one we have just used with the straight line. We consider a set of varied curves.

$$\begin{align} Y(x) = y(x) + \epsilon \eta(x) \end{align}$$

just as before. Then we have 
$$\begin{align} I(\epsilon) = \int^{x_2}_{x_1} F(x,Y, Y')\;dx\end{align}$$

and we want $(d/d\epsilon)I(\epsilon) = 0$ when $\epsilon = 0$. Remembering that $Y$ and $Y'$ are functions of $\epsilon$ and differentiating under the integral sign with respect to $\epsilon$, we get
$$\begin{align} \frac{dI}{d\epsilon}=\int^{x_2}_{x_1} \left(\frac{\partial F}{\partial Y}\frac{dY}{d\epsilon} + \frac{\partial F}{\partial Y'}\frac{dY'}{d\epsilon}\right)dx\end{align}$$

Which then gives us:
$$\begin{align} \frac{dI}{d\epsilon} = \int^{x_2}_{x_1} \left[\frac{\partial F}{\partial Y} \eta(x) + \frac{\partial F}{\partial Y'}\eta'(x)\right] dx \end{align}$$

We want $dI/d\epsilon=0$ at $\epsilon = 0$; recall that $\epsilon = 0$ means $Y = y$ then:
$$\begin{align} \left(\frac{dI}{d\epsilon}\right)_{\epsilon=0} = \int^{x_2}_{x_1} \left[\frac{\partial F}{\partial y} \eta(x) + \frac{\partial F}{\partial y'}\eta'(x)\right] dx \end{align}$$

Assuming that $y''$ is continuous, we can integrate the second term by parts:

$$\begin{align} \int^{x_2}_{x_1}\frac{\partial F}{\partial y'}\eta'(x) dx = \frac{\partial F}{\partial y'}\eta(x)\bigg|^{x_2}_{x_1} - \int^{x_2}_{x_1}\frac{d}{dx}\left(\frac{\partial F}{\partial y'}\right) \eta(x)\;dx \end{align}$$

The integrated term is zero as before because $\eta(x)$ is zero at $x_1$ and $x_2$. Then we have $$\begin{align} \left(\frac{dI}{d\epsilon}\right)_{\epsilon=0} = \int^{x_2}_{x_1}\left[\frac{\partial F}{\partial y} - \frac{d}{dx}\frac{\partial F}{\partial y'}\right] \eta(x) dx = 0 \end{align}$$

Since $\eta(x)$ is arbitrary we must have 
>$$\begin{align} \frac{d}{dx}\frac{\partial F}{\partial y'} - \frac{\partial F}{\partial y} = 0\end{align}$$

This is the Euler (or Euler-Lagrange) equation.

[[Example 3]]
