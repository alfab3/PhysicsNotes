## First Assumptions
We have two Hermitian operators $\hat q$ and $\hat p$ with commutator $$ \begin{gather}[\hat q, \hat p] = i\hbar \\ \hat H = H(\hat q, \hat p) \end{gather}$$ 
## Operators
$$\begin{gather} \hat a = \alpha \hat q + i \beta \hat p \;\;\; \text{Lowering Operator}\\  \hat a^\dagger = \alpha^*\hat q - i\beta^*\hat p \;\;\; \text{Raising Operator}\end{gather}$$

We select $\alpha \beta^* + \alpha^* \beta = 1/\hbar$  

$$\begin{gather} [\hat a, \hat a^\dagger] = \hbar(\alpha\beta^* + \alpha^*\beta) = 1\end{gather}$$

We write $\hat q$ and $\hat p$ as: 
$$\begin{gather} \hat q = \hbar (\beta\hat a^\dagger+\beta^*\hat a) \\ \hat p = i\hbar(\alpha\hat a^\dagger - \alpha^*\hat a) \end{gather}$$


## Number Operator
$$\begin{gather} \hat n = \hat a^\dagger\hat a \\ \hat n \ket{n} = n \ket{n} \;\;\; (n= 0,1,2,\ldots) \\ [\hat n, \hat a^\dagger] = \hat a^\dagger \;\;\;\; [\hat n, \hat a] = -\hat a \end{gather}$$
## Raising and Lowering Operator Properties
$$\begin{gather} \hat a \ket{0} = 0, \;\;\; \hat{a}\ket{n} = \sqrt{n}\ket{n-1} \;\;\; (n = 1,2,3,\ldots) \\ \hat a ^\dagger \ket{n} = \sqrt{n+1}\ket{n+1} \;\;\; (n=0,1,2,\ldots) \\ \\ \ket{n} = \frac{(\hat a^\dagger)^n}{\sqrt{n!}}\ket{0} \end{gather}$$

## General Harmonic Oscillator
$$\begin{gather} H = A\frac{\hat q^2}{2} + B \frac{\hat p^2}{2} \;\;\; (A >0, B>0) \end{gather}$$