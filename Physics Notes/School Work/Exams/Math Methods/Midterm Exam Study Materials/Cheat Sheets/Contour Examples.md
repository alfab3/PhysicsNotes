#### Example - Sector Contour

$$\begin{gather} f(x) = \int^\infty_0\frac{dx}{1+x^a} \end{gather}$$
##### Step 1: Solve for poles

$$\begin{gather} 1+x^a \Rightarrow x^a = -1 \Rightarrow x^a = e^{i\pi} \Rightarrow x = e^{i\pi/a}\end{gather}$$

##### Step 2: Define a Contour
![[sector contour.png]]

Sector length: $s = r\phi = Re^{i\theta} = e^{2i\pi/a}$
Define each segment:
1: $0 \to R$
2: $R \to R^{2\pi i/a}$
3: $R \to 0$

##### Step 3: Setup Contour Integral
>$$\begin{gather} \oint_\Gamma \frac{dx}{1+x^a} \Rightarrow \oint_\Gamma \frac{dx}{1+x^a} = \int_0^R \frac{dx}{1+x^a} + \int_2 \frac{dz}{1+z^a} + \int_R^0\frac{dz}{1+z^a}\end{gather}$$

Segment 1: 
Simple, just integrating over the real line, no change is necessary.

Segment 2:
Since this is an angular segment we must redefine $z$: 

>$$\begin{gather} z = Re^{i\theta} \Rightarrow dz  = iRe^{i\theta} d\theta \\ \lim_{R\to\infty}\int \frac{iRe^{i\theta}d\theta}{1 + Re^{ai\theta}} \approx \frac{R}{R^a} = \frac{1}{R^{a-1}} \to 0\end{gather}$$

Therefore: 

>$$\begin{gather} \int_2 \frac{dz}{1+z^a} \to 0 \end{gather}$$

Segment 3:
Similar to segment 1 but it is rotated. 

What is the rotation?
>$$\begin{gather} x \mapsto xe^{i\theta}e^{i\pi} = -xe^{i\theta} \end{gather}$$

>$$\begin{gather} \int_R^0\frac{dz}{1+z^a} \Rightarrow -e^{i\theta} \int^R_0 \frac{dx}{1+x^a} \end{gather}$$

So the integral is now:
$$\begin{gather} \int^R_0 \frac{dx}{1+x^a}(1-e^{2i\pi/a}) \end{gather}$$

##### Step 4: Evaluate Integral

$$\begin{gather} (1-e^{2i\pi/a})\int^\infty_0\frac{dx}{1+x^a} = 2\pi i \sum_{z_0}\text{Res}[\frac{1}{1+z^a}, e^{i\pi/a}]\\ \text{Res}[\frac{1}{1+z^a}, e^{i\pi/a}] = \lim_{z\to e^{i\pi/a}} \frac{z - e^{i\pi/a}}{1+z^a} = \lim\frac{z - e^{i\pi/a}}{z^{a-1}(z+z^{1-a})} = \frac{1}{ae^{i\pi(a-1)/a}} \\ =\frac{1}{a}e^{i\pi(1-a)/a} \\ \Rightarrow \int^\infty_0\frac{dx}{1+x^a} = \frac{2\pi ie^{i\pi(1-a)/a}}{a(1-e^{2\pi i/a})} \end{gather}$$