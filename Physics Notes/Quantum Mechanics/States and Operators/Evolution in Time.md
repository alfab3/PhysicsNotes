Any function of time can be expressed as a [[Taylor Series]]:

$$\begin{gather} \ket{\psi(t_0 + \tau)} = \ket{\psi(t_0)} + \tau \frac{d}{dt}\ket{\psi(t)}_{t=t_0} + \frac{\tau^2}{2}\frac{d^2}{dt^2} \ket{\psi(t}_{t=0} + \ldots + \frac{\tau^n}{n!} \frac{d^n}{dt^n} \ket{\psi(t)}_{t=t_0}\end{gather}$$

With the Taylor expansion for $e^x = 1 + x + \ldots + x^n/n! + \ldots$ one can see that:

$$\begin{gather} \ket{\psi(t_0+\tau)} = U(t_0,t_0+\tau)\ket{\psi(t)}_{t=t_0} \\ U(t_0,t_0 + \tau) = \exp\left\{\tau \frac{d}{dt}\right\} \end{gather}$$

$U(t_0, t_0 + \tau)$ is the evolution operator as it evolves the state forward or backward in time by an amount $\tau$ 

$$\begin{gather} U^\dagger(0,t)U(0,t) = \mathbb I \end{gather}$$
Which means $U$ is a Unitary operator ([[Unitary Operators and Transformations]]).

# Small Times
Define an operator $H$: 

$$\begin{gather} H(t) = i\hbar \frac{d}{dt} \\ H(t) \ket{\psi(t)} = i\hbar \frac{d}{dt}\ket{\psi(t)}\end{gather}$$
Then: 

$$\begin{gather} U(t,t+\tau) = e^{-iH\tau/\hbar} \end{gather}$$
