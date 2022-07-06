To derive the fact that integrating the [[Phase]] $e^{ikx}$ gives a [[Dirac Delta Function]], one can add a factor $e^{-\epsilon|x|}$ to the integrand and take the limit $\epsilon \to 0$. The proof then goes like

$$\begin{gather} \int^{\infty}_{-\infty} dx e^{ikx} = \int_{-\infty}^ 0 dx ^{\epsilon x +ikx} + \int_0^\infty e^{-\epsilon x +ikx}\Bigg|_{\epsilon\to 0} \\ = \frac{1}{\epsilon+ik}+\frac{1}{\epsilon-ik} \\ = \frac{2\epsilon}{\epsilon^2+k^2}\Bigg|_{\epsilon\to 0} \end{gather}$$

The r.h.s is clearly zero when $k\neq0$, but is infinity for k = 0. To see that this is proportional to $\delta(k)$, one need only integrate the function and se$$\begin{gather} \int ^{\infty}_{-\infty} dk \frac{2\epsilon}{\epsilon^2+k^2} = 2 \pi \delta(k)\end{gather}$$

To perform the above integral, one can use a trig substitution: $k = \epsilon\tan\theta$ 