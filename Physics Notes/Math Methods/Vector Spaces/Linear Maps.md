A linear map $A:V \rightarrow W$ is a function that satisfies:
1) $A(\ket{v}+\ket{w})$
2) $A(\lambda \ket{v}) = \lambda A(\ket{v})$

A linear map is completely specified by its action on a basis:

if $A\ket{v} = \ket{w}$, we have using compnents: 
$$w^\mu \ket{e_\mu} = A(v^\nu \ket{e_\nu})$$ 
and using the properties of linearity 
$$w^\mu \ket{e_\mu} = v^\nu A\ket{e_\nu}$$
and defining $A^\nu_\mu$ from $A\ket{e_\nu} = A^\nu_\mu \ket{e_\mu}$

We obtain:
$$w^\mu = A^\mu_\nu v^\nu$$