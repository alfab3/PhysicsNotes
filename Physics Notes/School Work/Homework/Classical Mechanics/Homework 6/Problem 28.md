# Statement of the System
The systems described by the [[Lagrangian]]

$$\begin{gather} \mathcal L = \frac{m_1}{2}\dot x_1^2 + \frac{m_2}{2}\dot x_2^2 - \frac{\kappa_{11}}{2}x_1^2 - \frac{\kappa_{22}}{2}x^2_2 - \frac{\kappa_{12}}{2}(x_1-x_2)^2 \end{gather}$$

are generically referred to as two coupled harmonic oscillators

## Part B
Problem: Find the [[Eigenfrequency]] and [[Eigenvectors]] of the [[Normal Modes]]

### Find Matrices
In a system such as this it is easy to just snag the different values but let's do it explicitly. 

For $\mathcal M$ we can use: 

$$\begin{gather} \frac{\partial \mathcal L}{\partial \dot{\vec  x_i}} \dot {\vec{x}}_i = \mathcal M\dot {\vec{x}}_i\end{gather}$$

Applying this to the Lagrangian we obtain:

$$\begin{gather} \frac{\partial \mathcal L}{\partial \dot{\vec  x_1}} \dot {\vec{x}}_1 =m_1\dot x_1, &\frac{\partial \mathcal L}{\partial \dot{\vec  x_2}} \dot {\vec{x}}_2 =m_2\dot x_2 \end{gather}$$

So our matrix becomes:

$$\begin{gather}\mathcal M = \begin{bmatrix} m_1 & 0\\ 0 & m_2 \end{bmatrix} \end{gather}$$

Now we need our $\mathcal K$ matrix:

We can rewrite the Potential term as:

$$\begin{gather} U = -\frac{1}{2}[(\kappa_{11}+\kappa_{12})x_1^2+(\kappa_{22}+\kappa_{12})x_2^2-2\kappa_{12}x_1x_2]\end{gather}$$

Notice how each term is now coupled to a term of $x_i$.

So now we can say:

$$\begin{gather} \mathcal K_{11} = \kappa_{11} + \kappa_{12}, &\mathcal K = \kappa_{22}+\kappa_{12}, &\mathcal K_{12}=\mathcal K_{21} = -\kappa_{12}\end{gather}$$

So our matrix takes the form:

$$\begin{gather} \mathcal K = \begin{bmatrix}  \kappa_{11} + \kappa_{12} & -\kappa_{12} \\ -\kappa_{12} & \kappa_{22} + \kappa_{12}   \end{bmatrix}  \end{gather}$$

Now we want to use the [[Characteristic Equation]]: 

$$\begin{gather}\det (\mathcal K - \omega^2 \mathcal M) = 0 \end{gather}$$

Where $\omega^2$ is our [[Eigenfrequency]]. We may also define it as $\lambda$ for simplicity. 

$$\begin{gather}\det (\mathcal K - \lambda \mathcal M) = 0 \end{gather}$$

First perform the operations, then take the determinant:

$$\begin{gather} a\lambda^2-b\lambda+c = 0 \\ a = m_1m_2 \\ b = m_1\kappa_{22}+m_2\kappa_{11}+\kappa_{12}(m_1+m_2) \\ c = \kappa_{11}\kappa_{22}+\kappa_{12}(\kappa_{11}+\kappa_{12})\end{gather}$$ 

To solve for $\lambda$, we use the quadratic equation:

$$\begin{gather} \lambda-{1,2} = \frac{-b\pm\sqrt{b^2-4ac}}{2a} & \omega_{1,2} = \sqrt{\lambda_{1,2}}\end{gather}$$