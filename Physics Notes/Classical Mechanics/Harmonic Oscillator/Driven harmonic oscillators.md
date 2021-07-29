Driven [[Harmonic Oscillator]]s are damped oscillators further affected by an externally applied force([[Force Newtonian Dynamics]]) $F(t)$

Newton's second law takes the form 
$$
F(t)-kx - c \frac{dx}{dt} = m \frac{d^2x}{dt^2}
$$
It is usually rewritten into the form 
$$
\frac{d^2x}{dt^2}+2\xi \omega_0\frac{dx}{dt} + \omega_0^2 x = \frac{F(t)}{m}
$$
This equation can be solved exactly for any driving force, using the solutions $z(t)$ that satisfy the unforced equation 
$$
\frac{d^2z}{dt^2} + 2 \xi \omega_0\frac{dz}{dt} + \omega^2_0 z = 0
$$
and which can be expressed as damped sinusoidal oscillations:
$$
z(t) = Ae^{-\xi \omega_0 t}sin(\sqrt{1-\xi^2}\omega_0 t + \phi)
$$
In the case where $\xi \leq 1$. The [[Amplitude]] $A$ and phase $\phi$ determine the behavior needed to match the initial conditions
