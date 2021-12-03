## 3.6)Solving for Green's Functions
### 3.6.1) General Process
1) Start with PDE
2) Determine the solution of the PDE using Fourier Transform
3) Plug the solution into the Fourier Transform
4) Plug in the inverse Fourier Transform
5) Solve integral(if possible)

#### Definition: Gaussian Integral Trick

>$$\begin{gather} \int^{\infty}_{-\infty} dke^{-ak^2+bk}=\int dke^{-a(k+\frac{b}{2a})^2+\frac{b^2}{4a}} \\ \tilde k = \sqrt{a}\left(k+\frac{b}{2a}\right) \\ \Rightarrow e^{b^2/4a}\frac{\sqrt{\pi}}{\sqrt{a}}\end{gather}$$


#### Example: Wave Equation
Consider the following PDE:

>$$\begin{gather} \frac{\partial \phi}{\partial t} = D\frac{\partial \phi^2}{\partial x^2} \end{gather}$$

Where 
>$$\begin{gather}\phi(x,t) = \frac{1}{2\pi}\int^\infty_{-\infty} dk \tilde \phi(k,t)e^{ikx}\end{gather}$$

Now we can utilize this form of the solution and plug into the PDE:

>$$\begin{gather} \frac{1}{2\pi}\int^\infty_{-\infty} dk \frac{\partial \tilde \phi}{\partial t}(k,t) = D\frac{1}{2\pi} \int^\infty_{-\infty} dk(-ik)^2\tilde\phi(k,t) \\ \frac{\partial \tilde \phi}{\partial t} = - Dk^2\tilde\phi \\ \tilde\phi (k,t) = \tilde\phi(k,t=0)e^{-Dk^2t}\end{gather}$$

Now we need to find $\phi(x,t)$ by using the inverse transform:

>$$\begin{gather} \phi(x,t) = \frac{1}{2\pi} \int^\infty_{-\infty} dk \tilde \phi(k,t=0)e^{ikx-Dk^2t}\\ \Rightarrow \phi(x,t) = \int^{\infty}_{-\infty}d\xi f(\xi)\int^\infty_{-\infty}dke^{ik(x -\xi) - Dk^2t}\end{gather}$$

Utilizing the Gaussian Integration trick: 

>$$\begin{gather} \frac{1}{\sqrt{4\pi Dt}}e^{-\frac{1}{4Dt}(x-\xi)^2} \\ G(x-\xi,t)\equiv \frac{1}{\sqrt{4\pi Dt}}e^{-\frac{1}{4Dt}(x-\xi)^2} \\ \phi(x,t) = \int^\infty_{-\infty}d\xi\phi(\xi,t=0)G(x-\xi,t)\end{gather}$$

Where G is Green's function.