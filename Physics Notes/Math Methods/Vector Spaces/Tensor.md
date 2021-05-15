A Tensor of type $(p,q)$ over a vector space ([[Linear Vector Spaces]])$V$ is an element of 
$$V \otimes V \otimes ... \otimes V \otimes V^* \otimes V^* \otimes ... \otimes  V^* $$ 
Where $V$ happens p times and $V^*$ happens q times. 
(1,0) tensor is a vector
(0,1) tensor is a covector

For instance, consider a (0, z) tensor $g \in V^* \otimes V^*$, then, by definition, there are some $\bra{w}$ and $\bra{x}$ such that 
$$g = \sum^K_{i = 1} \bra{w_i} \otimes \bra{x_i}$$ 
Now, $g$ can be seen as a map ([[Linear Maps]]) $\hat{g}$ from $V$ to $V^*$, defined as 
$$\hat{g}\ket{x} = \sum^n_{i=1} \braket{w_i|x} \otimes \bra{x_i} = \sum^k_{i=1} \braket{w_i | x} \bra{x_i} $$
But also, $g$ can be seen as a bilinear map $$\tilde{g}: V \otimes V \rightarrow F: \tilde{g} \ket{v} \otimes \ket{w} = \sum^k_{i=1} \braket{w_i|v} \braket{x_i|w}$$

To sum up; a $(0,z)$ tensor can be seen as:
1) a linear map $V \rightarrow V^*$
2) a bilinear map $V \times V \rightarrow F$

In a similar fashion, a $(\hat{i},1)$ tensor $A \in V \otimes V^*$ can be seen as a linear operator 
$$V \rightarrow \; or \; V^* \otimes V \rightarrow F \; or \; V^* \rightarrow V^*$$
In components, we have 
$$A = A^\mu_\nu \ket{e_\mu} \bra{\theta^\nu}$$
so that 
$$A\ket{x} = A^\mu_\nu \ket{e_\mu} (\braket{\theta^\nu | x}) = A^\mu_\nu \ket{e_\mu} (\braket{\theta^\nu|x^\alpha|e_\alpha}) = A^\mu_\nu x^\alpha \ket{e_mu} \delta^\nu_\alpha = A^\mu_\nu x^\nu \ket{e_\mu}$$