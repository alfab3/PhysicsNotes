#### Example 1: First Order $\omega(x) = 1$
Find adjoint of the Linear Differential Operator: $\mathcal L = -i \frac{d}{dx}$ with $\omega(x) = 1$

>$$\begin{gather} \overline{u}(\mathcal L v) = \overline u\left(-i\frac{d}{dx} v\right) = \left(i\frac{d}{dx} \overline{u}\right)v - i\frac{d}{dx}(\overline uv) = \overline{\left(-i\frac{d}{dx} u \right)} v + \frac{d}{dx}(-i \ \overline{u} v) \\ \mathcal L^\dagger = -i\frac{d}{dx} =\mathcal L^\dagger \\ Q[u,v] = -i \ \overline u v\end{gather}$$

Therefore $\mathcal L = -i\frac{d}{dx}$ is formally self-adjoint

#### Example 2: Second Order Diff eq $\omega(x) = 1$
>$$\begin{align} \mathcal L = p_0(x)\frac{d^2}{dx^2} + p_0\frac{d}{dx} + p_2(x) \end{align}$$

We use a similar approach and find that:

>$$\begin{gather} \mathcal L^\dagger = p_0(x)\frac{d^2}{dx^2}+(2p_0'(x)-1)\frac{d}{dx} + [p_o''(x) - p_1'(x) + p_2(x)] \end{gather}$$

Formal self-adjointness with $\omega(x)$ of above operator is only if $p_0'(x) = p_1(x)$, $p_0''(x) = p_1'(x)$.

$\mathcal L$ is self-adjoint with $\omega(x) = 1$
>$$\begin{gather} \mathcal L = \frac{d}{dx}\left(p_0 \frac{d}{dx}\right) + p_2(x)\end{gather}$$

This is called the Sturm-Liouville Operator

Any 2nd order diff op is formally-self - adjoint with a weight function: 

>$$\begin{gather} \omega(x) = \frac{1}{p_0(x)} e^{\int^x_a\left(\frac{p_1(x')}{p_0(x')}\right)dx'}\end{gather}$$

#### Example 3: Momentum Operator $\omega(x) > 0$

Consider the momentum linear operator: $\mathcal L -i \frac{d}{dx}$ for functions on the interval $x \in [a,b]$. Find the Adjoint operator $\mathcal L$

Start with the Lagrange identity:

>$$\begin{gather} \omega(x)(\overline u \mathcal L v - v\overline{\mathcal L u}) = \frac{d}{dx} Q(u,v) \\ \omega \overline u\left(- i \frac{d}{dx}\mathcal L v\right) = \omega \overline u\left( -i \frac{d}{dx}v\right)\end{gather}$$

Now we "move" the derivative operator to $\overline u$

>$$\begin{gather} \omega \overline u \left(-i \frac{d}{dx} v\right) = -i\frac{d}{dx}(\omega \overline u v)  + v i \frac{d}{dx}(\omega \overline u) = -i\frac{d}{dx}(\omega \overline u v) + \omega v i \frac{d}{dx}\overline u + \overline u v i \frac{d}{dx}\omega \end{gather}$$

Let us now write $\mathcal L^\dagger = \mathcal L^\dagger_1 + \mathcal L_2^\dagger$

such that: 
>$$\begin{gather}\omega v i \frac{d}{dx}\overline u + \overline u v i \frac{d}{dx} = \omega v \overline{\mathcal L^\dagger_1 u} + \omega v \overline{\mathcal L^\dagger_2 u}  \end{gather}$$

It is easy to see that: 
>$$\begin{gather} \overline{\mathcal L^\dagger_1 u} = i\frac{d}{dx} \overline u = \overline{-i \frac{d}{dx} u} \Rightarrow \mathcal L^\dagger_1 = -i\frac{d}{dx} = \mathcal L \end{gather}$$

Now we solve for the second term:
>$$\begin{gather} \omega v \overline{\mathcal{L}^\dagger u} = \overline{u}v i \frac{d}{dx} \omega = \omega v i \frac{1}{\omega} \frac{d\omega}{d x}\overline{u} = \omega v \left(\overline{-i \frac{1}{\omega}\frac{d\omega}{d x} u}\right) \\ \overline{\mathcal L^\dagger_2 u} = \overline{-i\frac{1}{\omega}\frac{d\omega}{dx}u}\\ \mathcal L_2^\dagger = - i\frac{1}{\omega}\frac{d\omega}{dx} = -i \frac{d}{dx}(\ln \omega) \\ \mathcal L^\dagger = -i\frac{d}{dx} - i\frac{d}{dx}\ln\omega \end{gather}$$

#### Example 4: Second Order Operator
>$$\begin{align} \mathcal L = p_0(x)\frac{d^2}{dx^2} + p_0\frac{d}{dx} + p_2(x) \end{align}$$

With the corresponding weight function: 
>$$\begin{gather} \omega(x) = \frac{1}{p_0(x)} e^{\int^x_a\left(\frac{p_1(x')}{p_0(x')}\right)dx'}\end{gather}$$

Begin with 
>$$\begin{gather} \omega\left(\overline{u} \mathcal L v - v \overline{\mathcal L^\dagger u}\right) = - \frac{d}{dx} Q(u,v) \end{gather}$$

with $\mathcal L^\dagger = \mathcal L$