## Poynting Vector
$$\begin{gather} \vec S(t) = \frac{1}{\mu_0} \vec E_a \times \vec B_a = \epsilon_0 c E^2_a \hat n _{\text{ret}} = \epsilon_0 c \left(\frac{q}{4\pi\epsilon_0}\right)^2\left|\frac{\hat n [(\hat n -\vec \beta) \times \dot{\vec{\beta}}]}{cg^3R}\right|^2_{\text{ret}} \hat n_{\text{ret}}\end{gather}$$

Rate at which energy flows through solid angle $d\Omega$ of a distant enclosing sphere of radius $R$: 
$$\begin{gather} \frac{dP(t)}{d\Omega} = \frac{dU}{dtd\Omega} = R^2\vec S(t) \cdot \hat n_{\text{ret}} \end{gather}$$
For retarded times:

$$\begin{gather} \frac{dP(t_{\text{ret}})}{d\Omega} = \frac{dU}{dt_{\text{ret}}d\Omega} = g_{\text{ret}}R^2\vec S(t) \cdot \hat n _\text{ret} = \frac{q^2}{16\pi^2\epsilon_0c}\frac{|\hat n \times[(\hat n - \vec \beta)\times \dot{\vec{\beta}}]|^2}{(1-\hat n \cdot \vec \beta)^5} \end{gather}$$
## Non-relativistic Motion
When the particle acceleration $\vec a = c \dot{\vec{\beta}}$  does not vanish

$$\begin{gather} \frac{dP}{d\Omega} = \frac{\mu_0 q^2}{16\pi^2 c}|\hat n \times (\hat n \times \vec a)| = \frac{\mu_0 q^2}{16\pi^2 c}|\hat r \times \vec a|^2 = \frac{\mu_0q^2a}{16 \pi^2 c}sin^2\theta\end{gather}$$
## Acceleration || Velocity
Gives rise to azimuthal symmetry around their common direction 

$$\begin{gather} \frac{dP}{d\Omega} \Bigg \vert_{|\vert} = \frac{\mu_0 q^2}{16 \pi^2 c} \frac{a^2 \sin^2 \theta}{(1-\beta\cos\theta)^5} \end{gather}$$
Bremsstrahlung - braking radiation, the case when  a < 0.

## Acceleration $\perp$ Velocity
$$\begin{gather} \frac{dP}{d\Omega}\Bigg|_\perp = \frac{\mu_0 q^2 a^2}{16 \pi^2 c} \frac{1}{(1-\beta \cos\theta)^3}\left[1 - \frac{\sin^2\theta \cos^2\phi}{\gamma^2(1-\beta\cos\theta)^2}\right]\end{gather}$$

## Larmor's Formula
$$\begin{gather} P =\frac{1}{4\pi\epsilon_0} \frac{2q^2}{3c^3}\gamma^6 \left[a^2-\left(\frac{\vec v \times \vec a}{c}\right)^2\right]_\text{ret} \end{gather}$$ 