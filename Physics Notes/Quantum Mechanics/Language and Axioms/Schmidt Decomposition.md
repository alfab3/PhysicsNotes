Consider a system split into two subsystems, $I$ and $II$. With a general choice of ONBs [[Orthonormal Basis]] in the [[Hilbert Space]]s of the subsystems $I$ and $II$, an expansion of any pure state $\ket{\psi}$ of our system has the generic form: 

$$\begin{gather}\ket{\psi} = \sum_{nm} c_{nm} \ket{e_{nm}} = \sum_{nm}c_{nm}\ket{e_n^{(I)}}\ket{e_m^{(II)}} \end{gather}$$

There is, however, a very special choice of orthonormal sets of vectors in two subsystems, $\{\ket{\phi_n^{(I)}}\}$ and $\{\ket{\phi_n^{(II)}}\}$ dictated by particular form of the pure state $\ket{\psi}$. With this special choice one has 

$$\begin{gather} \ket{\psi} = \sum_na_n\ket{\psi^{(I)}_n}\ket{\psi^{(II)}_n} \end{gather}$$
In mathematics the representation is known as Schmidt decomposition. It has quite important physical implications. Namely for the two [[Reduced Density Matrices]] it yields. 
$$\begin{gather}\hat \rho ^{(I)}=\sum_n|a_n|^2\ket{\phi_n^{(I)}}\bra{\phi_n^{(I)}} & \hat \rho^{(II)}=\sum_n|a_n|^2\ket{\phi_n^{(II)}}\bra{\phi_n^{(II)}}\end{gather}$$ 
revealing an instructive fact that, despite all possible qualitative and quantitative differences between the two subsystems - including different dimensions of [[Hilbert Space]]s the two reduced density matrices always feature remarkable correspondence between their [[Eigenvectors]], with the same [[Eigenvalues]] given by the squares of absolute values of coefficients $a_n$. 

The proof of Schmidt decomposition is also very physical in the sense that it utilizes the mathematical structure known in physics as reduced density matrix. Without loss of generality we assume that the dimension of the Hilbert space of subsystem $I$ is not larger than that of subsystem $II$(otherwise, swap $I$ and $II$. Given the pure state $\ket{\psi}$, construct the reduced density matrix $$\begin{gather} \hat\rho = \text{Tr}^{(II)} \hat\rho & \hat \rho =\ket{\psi}\bra{\psi}\end{gather}$$

Let $\{\ket{\phi^{(I)}_n}\}$ be an ONB of eigenvectors of $\hat \rho^{(I)}$. Then we have: 

$$\begin{gather} \ket{\psi} = \sum_n\ket {\phi^{(I)}_n}\ket{\varphi_n^{(II)}} \end{gather}$$

where $\{\ket{\phi_n^{(II)}}\}$ are certain states of subsystem $II$. Correspondingly
$$\begin{gather}\hat\rho = \sum_{n_1n_2} \ket{\phi^{(I)}_{n_1}}\ket{\varphi^{(II)}_{n_1}}\bra{\varphi^{(II)}_{n_2}}\bra{\phi^{(I)}_{n_2}} \\ \hat\rho^{(I)} = \text{Tr}^{(II)}\hat \rho = \sum_{n_1n_2} \ket{\phi^{(I)}_{n_1}}\braket{\varphi^{(II)}_{n_2}|\varphi^{(II)}_{n_1}}\bra{\phi_{n_2}^{(I)}}  \end{gather}$$

So far, we have used only the fact that $\{\ket{\phi_n^{(I)}}\}$ is a certain ONB in the [[Hilbert Space]] of the subsystem $I$. Now recall that the vectors $\{\ket{\phi^{(I)}_n}\}$ are eigenvectors of $\hat \rho ^{(I)}$, so that all the $n_1 \neq n_2$ terms in the above equation have to be identically equal to zero: 

$$\begin{gather} \hat \rho^{(I)} = \sum_n \ket{\phi^{(I)}}\braket{\varphi_n^{(II)}|\varphi_n^{(II)}}\bra{\phi^{(I)}_n} \end{gather}$$

This brings us to 
$$\begin{gather}\braket{\varphi^{(II)}_{n_2}|\varphi^{(II)}_{n_1}} = 0 & \text{if} & n_1 \neq n_2 \end{gather}$$

and thus: 

$$\begin{gather}\ket{\phi^{(II)}_n} = \frac{\ket{\varphi^{(II)}_n}}{\sqrt{\braket{\varphi_n^{(II)}|\varphi_n^{(II)}}}} & a_n = \sqrt{\braket{\varphi_n^{(II)}|\varphi_n^{(II)}}}\end{gather}$$

