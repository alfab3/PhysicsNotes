## Poynting Vector
$$\begin{gather} \vec S(t) = \frac{1}{\mu_0} \vec E_a \times \vec B_a = \epsilon_0 c E^2_a \hat n _{\text{ret}} = \epsilon_0 c \left(\frac{q}{4\pi\epsilon_0}\right)^2\left|\frac{\hat n [(\hat n -\vec \beta) \times \dot{\vec{\beta}}]}{cg^3R} \right|^2_{\text{ret}} \hat n_{\text{ret}} \end{gather}$$

Rate at which energy flows through solid angle $d\Omega$ of a distant enclosing sphere of radius $R$: 

$$\begin{gather} \frac{dP(t)}{d\Omega} = \frac{dU}{dtd\Omega} = R^2\vec S(t) \cdot \hat n_{\text{ret}} \end{gather}$$
For retarded times:
(Note: $P' = P(t_\text{ret}) = (1- \beta\cdot\hat n)$, The lecture notes, Jackson, and Zangwill all use different notation)
$$\begin{gather} \frac{dP(t_{\text{ret}})}{d\Omega} = \frac{dU}{dt_{\text{ret}}d\Omega} = g_{\text{ret}}R^2\vec S(t) \cdot \hat n _\text{ret} = \frac{q^2}{16\pi^2\epsilon_0c}\frac{|\hat n \times[(\hat n - \vec \beta)\times \dot{\vec{\beta}}]|^2}{(1-\hat n \cdot \vec \beta)^5} \\ \\ P' = \frac{2q^2}{3c} \left[\frac{\alpha^2 - |\vec \beta \times \vec \alpha|^2}{(1-\beta^2)^3}\right] = \frac{2q^2}{3c} \left[\frac{\alpha^2(1-\beta^2)+(\vec \alpha \cdot\vec \beta)^2}{(1-\beta^2)^3}\right]  \end{gather}$$
## Non-relativistic Motion ($\beta \ll 1$)
When the particle acceleration $\vec a = c \dot{\vec{\beta}}$  does not vanish

$$\begin{gather} \frac{dP}{d\Omega} = \frac{\mu_0 q^2}{16\pi^2 c}|\hat n \times (\hat n \times \vec a)| = \frac{\mu_0 q^2}{16\pi^2 c}|\hat r \times \vec a|^2 = \frac{\mu_0q^2a^2}{16 \pi^2 c}sin^2\theta \;\; \text{(SI)} \\ \\ \frac{dP}{d\Omega} = \frac{ q^2}{4\pi c}|\hat n \times (\hat n \times \vec a)| = \frac{ q^2}{4\pi c}|\hat r \times \vec a|^2 = \frac{q^2a^2}{4 \pi c}sin^2\theta \;\; \text{(Gaussian)} \\ \\ P = \frac{1}{4 \pi \epsilon_0} \frac{2q^2|\vec a_\text{ret}|^2}{3c^3} \;\; \text{(SI)} \\ \\ P =\frac{2q^2|\vec a_\text{ret}|^2}{3c^3} \;\; \text{(Gaussian)} \end{gather}$$
## Acceleration || Velocity
Gives rise to azimuthal symmetry around their common direction 

$$\begin{gather} \frac{dP'}{d\Omega} \Bigg \vert_{|\vert} = \frac{\mu_0 q^2}{16 \pi^2 c} \frac{a^2 \sin^2 \theta}{(1-\beta\cos\theta)^5} \;\; \text{(SI)} \\ \frac{dP'}{d\Omega} \Bigg \vert_{|\vert} = \frac{q^2}{4 \pi c} \frac{a^2 \sin^2 \theta}{(1-\beta\cos\theta)^5}  \;\; \text{(Gaussian)} \end{gather}$$
Bremsstrahlung - braking radiation, the case when  a < 0. Note: Positive or negative acceleration does not matter, since the acceleration term is is squared. 

#### Non-Relativistic Limit $\beta \to 0$ 
![[Screenshot from 2022-05-05 11-32-23.png]]

#### Ultra-Relativistic Limit $\beta \to 1$ 
![[Screenshot from 2022-05-05 11-36-33.png]]

#### For Varying Values of $\beta$
![[Screenshot from 2022-05-05 11-38-27.png]]

#### Total Power
$$\begin{gather} P' = \frac{2}{3}\frac{q^2a^2}{c^3} \gamma^6 \;\; \text{(Gaussian)} \end{gather}$$

## Acceleration $\perp$ Velocity (Relativistic Circular Motion, Synchotron) 

![[Screenshot from 2022-05-05 11-52-35.png]]

![[Screenshot from 2022-05-05 11-57-29.png]]


$$\begin{gather} \frac{dP'}{d\Omega}\Bigg|_\perp = \frac{\mu_0 q^2 a^2}{16 \pi^2 c} \frac{1}{(1-\beta \cos\theta)^3}\left[1 - \frac{\sin^2\theta \cos^2\phi}{\gamma^2(1-\beta\cos\theta)^2}\right] \;\; \text{(SI)} \\ \frac{dP'}{d\Omega} \Bigg|_\perp = \frac{q^2 a^2}{4 \pi c} \frac{1}{(1-\beta \cos\theta)^3}\left[1 - \frac{\sin^2\theta \cos^2\phi}{\gamma^2(1-\beta\cos\theta)^2}\right] \;\; \text{(Gaussian)} \\ \\ P' = \frac{2}{3}\frac{q^2a^2}{c^3} \gamma^4 \;\; \text{(Gaussian)}\end{gather}$$

## Larmor's Formula and Relativistic Generalization 
$$\begin{gather} P' =\frac{2}{3}\frac{e^2}{m^2c^3} \left(\frac{d\vec p}{dt} \cdot \frac{d\vec p}{dt}\right)  \\ \\ P= - \frac{2}{3} \frac{e^2}{m^2 c^3} \left(\frac{dp_\mu}{d\tau} \frac{dp^\mu}{d\tau}\right) \\ \\ d\tau = dt/\gamma\\  \\ E = \gamma mc^2 \;\;\; \vec p = \gamma m\vec v \\ \\ P' = \frac{1}{4\pi \epsilon_0} \frac{2q^2}{3c} \gamma^6 \left[\dot \beta^2 - (\vec \beta \times \dot{\vec{\beta}})^2\right]_\text{ret} \;\; \text{(SI)} \\ \\ P' = \frac{2q^2}{3c} \gamma^6 \left[\dot \beta^2 - (\vec \beta \times \dot{\vec{\beta}})^2\right]_\text{ret} \;\; \text{(Gaussian)}\end{gather}$$ 
#### Transverse Acceleration $( \vec \beta \cdot \vec \alpha = 0)$ 
$$\begin{gather} P' = \frac{2}{3}\gamma^2 \frac{q^2}{m^2c^3}\left(\frac{d\vec p}{dt}\right)^2 \end{gather}$$
#### Longitudinal Acceleration $(\vec \beta || \vec \alpha)$ 
$$\begin{gather} P' = \frac{2}{3} \frac{q^2}{m^2c^3}\left(\frac{d\vec p}{dt}\right)^2 \end{gather}$$
