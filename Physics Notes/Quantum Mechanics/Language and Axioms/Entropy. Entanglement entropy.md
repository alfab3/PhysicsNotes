For a density matrix $\hat \rho$, the quantity 

$$\begin{gather} S = - \sum_jw_j\ln w_j \equiv - \text{Tr}\hat \rho \ln \hat \rho \end{gather}$$

is called (von Neumann) entropy. The idea of this definition is a combination of the purely statistical notion of von Neumann entropy characterizing a distribution with the set of probabilities $\{w_j\}$ and the statistical interpretation of a mixed states in terms of the eigenvalues $\{w_j\}$ of the [[Density Matrix]]. There exist alternative entropies. For example, the so-called Renyi entropy plays an important role in quantum information. What is special about von Neumann entropy is its additivity for independent distributions - and in particular for disentangled density matrices of subsystems: 

$$\begin{gather}\hat \rho =\hat \rho^{(I)} \hat \rho^{(II)} & \Rightarrow & S = S^{(I)} + S^{(II)} \end{gather}$$

von Neumann entropy plays absolutely central role in thermodynamics. That is why in physics, the default meaning of the term "entropy" is the von Neumann entropy. 

The entanglement between two subsystems in a pure global state is characterized by the so-called entanglement entropy-the von Neumann entropy of the reduced density matrix: 

$$\begin{gather} S_{\text{entang}} = - \text{Tr}\hat\rho^{(I)}\ln\hat\rho^{(I)} = - \text{Tr}\hat\rho^{(II)}\ln\rho^{(II)}=-\sum_n|a_n|^2\ln|an|^2 \end{gather}$$