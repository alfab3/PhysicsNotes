## Dirac Delta Function

The identity operator in $\infty$-dim space is the Dirac-delta "function"

>$$\begin{gather}I\{f(x)\} = \int^b_a \delta(x-y) f(y)dy = f(x) \end{gather}$$

Derivative of the Delta Function: $\frac{d}{dx}\delta(x)$ 
>$$\begin{gather} \int^b_a\left[\frac{d}{dx} \delta(x-y) \right]f(y) dy = -\int^b_a f(y) \frac{d}{dy}\delta(x-y) = -\delta(x-y)f(y)\Bigg|^b_a + \int^b_a f'(y) \delta(x - y) \\ = f'(x)\end{gather}$$

Explanation of the first step:
>$$\begin{gather} \frac{d}{dx}\delta(x-y) = \frac{d}{d(x-y)}\delta(x-y)\frac{d(x-y)}{dx} = \delta'(x-y) \\ \frac{d}{dy}\delta(x-y) = \frac{d}{d(x-y)}\delta(x-y)\frac{d(x-y)}{dx} = -\delta'(x-y) \\ \frac{d}{dx}\delta(x-y) = -\frac{d}{dy}\delta(x-y)\end{gather}$$

Example:
Consider the Kernels:

>$$\begin{gather}K(x,y) = c_2(y)\delta''(x-y) + c_1(y)\delta'(x-y)+c_0(y)\delta(x-y) \\G(x,y) = c_2(x)\delta''(x-y) + c_1(x)\delta'(x-y)+c_0(x)\delta(x-y)\end{gather}$$
where $c_i(x)$ are twice differentiable in the interval $x \in [a,b]$

Consider $\delta(x-y)$ as a generalized function of the variable x, we have that:

>$$\begin{gather}\delta'(x-y) = \frac{d}{dx}\delta(x-y) = -\frac{d}{dy}\delta (x-y) \\ \delta''(x-y) = \frac{d^2}{dx^2}\delta(x-y) = \frac{d^2}{dy^2}\delta(x-y)\end{gather}$$

Therefore:
>$$\begin{gather} \int^b_a \delta''(x-y) f(y)c_s(y)dy = \int^b_a \frac{d^2}{dy^2}\delta(x-y) f(y)c_s(y)dy \\ = -\int^b_a\frac{d}{dy}\delta(x-y)\frac{d}{dy}[f(y)c_2(y)]dy = [f(x)c_2(x)]''\end{gather}$$

Whereas:
>$$\begin{gather} \int^b_a \delta''(x-y) f(y)c_2(x)dy = \int^b_a \frac{d^2}{dy^2}\delta(x-y) f(y)c_2(x)dy \\ = -\int^b_a\frac{d}{dy}\delta(x-y)\frac{d}{dy}[f(y)c_2(x)]dy = f(x)''c_2(x)\end{gather}$$

Now for 1st derivative:

>$$\begin{gather}\int^b_a \delta'(x-y)f(y)c_1(y)dy = -\int^b_a\frac{d}{dy}\delta(x-y)f(y)c_1(y)dy \\ = \int^b_{y=a}\delta(x-y)\frac{d}{dy}[f(y)c(y)]dy = [f(x)c_1(x)]' \\ \int^b_a \delta'(x-y)f(y)c_1(x)dy = -\int^b_a\frac{d}{dy}\delta(x-y)f(y)c_1(x)dy \\ = \int^b_{y=a}\delta(x-y)\frac{d}{dy}[f(y)c(x)]dy = f(x)'c_1(x)\end{gather}$$

>Finally: $$\begin{gather} \int^b_a c_0(y)\delta(x-y)f(y)dy = c_0(x)f(x) \\ \int^b_a c_0(x)\delta(x-y)f(y)dy = c_0(x)f(x) \end{gather}$$

Therefore: 

>$$\begin{gather} \int^b_aK(x,y)f(y)dy = [c_2(x)f(x)]'' + [f(x)c_1(x)]' + c_0(x)f(x) \\ \int^b_a G(x,y)f(y)dy = f(x)''c_2(x) + f(x)'c_1(x) + c_0(x)f(x)\end{gather}$$

