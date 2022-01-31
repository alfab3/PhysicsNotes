### 3.2.2) Integration by parts technique

Consider an operator $\mathcal L = -\frac{d^2}{dx^2}$

We want to apply this to Lagrange's identity, where it will be acting on $v$ and we are going to "move" the operator to $u$:

>$$\begin{gather} \int \overline{u} \mathcal L v dx= -\int \overline{u} \frac{d^2v}{dx^2} dx\end{gather}$$

Now we set $u = u$ and $v = \frac{d}{dx}v$ and apply integration by parts which is defined as:

>$$\begin{gather} \int udv = uv - \int vdu  \end{gather}$$

Applying this to the right hand side of our above equation 
>$$\begin{gather} -\int \overline{u} \frac{d^2v}{dx^2} dx = \overline{u}\frac{dv}{dx} - \int \frac{dv}{dx}\frac{d\overline{u}}{dx}dx\end{gather}$$

Now we must apply the integration by parts technique once more. $\overline{u} = \frac{d\overline{u}}{dx}$ and $v = v$

>$$\begin{gather} \overline{u}\frac{dv}{dx} - \int \frac{dv}{dx}\frac{d\overline{u}}{dx}dx = \overline{u}\frac{dv}{dx} + \frac{d\overline{u}}{dx}v - \int \frac{d^2u}{dx^2}vdx \\ =-\left(\overline{u} \frac{dv}{dx} - \frac{d\overline{u}}{dx}v\right)+\int v\mathcal L^\dagger\ \overline{u}dx \end{gather}$$

We have arrived at the (formal) adjoint operator.

Now let us consider a weight function $\omega(x) > 0$

Consider the momentum operator case: 

>$$\begin{gather} \mathcal L = -i\frac{d}{dx} \end{gather}$$

Utilizing Lagrange's identity we can see that:

>$$\begin{gather} \int \omega \overline{u} \mathcal L v = \int \omega \overline{u} \left(-i\frac{d}{dx} v\right) \end{gather}$$

Using integration by parts we define $u = \omega u$ and $v = v$

>$$\begin{gather}\int \omega \overline{u} \left(-i\frac{d}{dx} v\right) = -i\omega \overline{u} v + \int iv\frac{d}{dx}(\overline{u} \omega) \end{gather}$$

Now this can be written in derivative form as:
>$$\begin{gather} \omega \overline{u} \left(-i\frac{d}{dx} v\right) = -i\frac{d}{dx}(\omega \overline{u} v) +  iv\frac{d}{dx}(\overline{u} \omega) \end{gather}$$

Since $\omega$ is dependent on $x$ then we must apply product rule:

>$$\begin{align} -i\frac{d}{dx}(\omega \overline{u} v) +  iv\frac{d}{dx}(\overline{u} \omega) = -i\frac{d}{dx}(\omega \overline{u} v) + iv\omega\frac{d}{dx}(\overline{u}) + iv\overline{u}\frac{d}{dx}(\omega) \end{align}$$

The integration by parts is complete.