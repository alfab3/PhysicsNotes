At $\omega \to \omega_0$ the amplitude of the solution becomes arbitrarily large. This is the phenomenon of resonance. Let us trace the initial period of evolution from some small amplitude at $t = 0$ to a large amplitude. The relevant solution is $$\begin{align} \eta(t) = \frac{a}{\omega_0^2 - \omega^2}[\cos \omega t - \cos\omega_0 t ]\end{align}$$

At small enough time, such that $$\begin{align} t \ll 1/|\omega_0 - \omega|\end{align}$$

we have $\cos \omega t \approx \cos \omega_0 t$ and we can take advantage of Taylor expansion:
$$\begin{align} \cos(\omega t) = \cos(\omega_0 t) + (\omega_0 - \omega)t\sin\omega_0t+... \end{align}$$

We get:

$$\begin{align} \eta(t) \approx \frac{at}{2\omega_0}\sin\omega_0t \end{align}$$

To analyze the close-to-resonance solution at larger times we write:
$$\begin{align}\eta(t) = \frac{a}{\omega_0^2-\omega^2}\text{Re} [e^{i\omega t}-e^{i\omega_0t}] \end{align}$$

and note that: 
$$\begin{align} e^{i\omega t}-e^{i\omega_0t} = 2ie^{i(\omega+\omega_0)t/2}\sin\frac{\omega - \omega_0}{2}t
\end{align}$$

Take the real part:

$$\begin{align}\eta(t) = \frac{2a}{\omega_0^2 - \omega^2}\sin\frac{\omega_0-\omega}{2}t\sin\frac{\omega +\omega_0}{2}t \end{align}$$

We are interested in the case $|\omega_0 - \omega| \ll \omega_0$. 


Here the magnitude of the first sine can be viewed as a slowly varying time independent amplitude modulating the sinusoidal oscillation of the normal mode, this phenomenon is known as _beats_