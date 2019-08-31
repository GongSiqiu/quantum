# Quantum information with Gaussian states

## Introduction

### Phase space representation and definition of Gaussian states

Consider the single-mode field. We have photon-number operator, N̂ . Any
Fock state $$|l\rangle$$ is an eigen-state of photon-number operator, i.e., $$\hat{N} |l\rangle = l|l\rangle$$.Also, we have creation operator $$a^†$$ and annihilation operator $$a$$
and $$\hat{N} = a^† a$$
$$
a^\dagger a|l\rangle=l|l\rangle
$$
$$
a^\dagger|l\rangle =\sqrt{l+1}|l+1\rangle
$$
$$
a|l\rangle=\sqrt{l}|l-1\rangle
$$

$$
[a,a^\dagger]=aa^\dagger-a^\dagger a=1
$$

$$
|l\rangle=\frac{{a^\dagger}^l}{\sqrt{l!}}|0\rangle
$$

$$
|\chi\rangle=f(a^\dagger)|0\rangle
$$

Let $$\hat{x}_k$$ and $$\hat{p}k$$ denote the ‘position’ and ‘momentum’ operators associated with
the $$k$$th mode, respectively (k = 1, 2, · · · , n).
$$
\begin{aligned} \hat{x}_{k} &=\sqrt{\frac{1}{2 \omega_{k}}}\left(a_{k}+a_{k}^{\dagger}\right) \\ \hat{p}_{k} &=-i \sqrt{\frac{\omega_{k}}{2}}\left(a_{k}-a_{k}^{\dagger}\right) \end{aligned}
$$
Defing $$R=\left(R_{1}, R_{2}, \cdots, R_{2 n}\right)^{T}=\left(\omega_{1}^{1 / 2} \hat{x}_{1}, \omega_{1}^{-1 / 2} \hat{p}_{1}, \cdots, \omega_{n}^{1 / 2} \hat{x}_{n}, \omega_{n}^{-1 / 2} \hat{p}_{n}\right)^{T}$$

these canonical commutation relations (CCRs) can be written compactly as $$[R_j,R_k]=iJ_{jk}$$.Here,$$J=\oplus^n_{j=1}J_1$$ with 
$$
J_{1}=\left(\begin{array}{cc}{0} & {1} \\ {-1} & {0}\end{array}\right)
$$
An n−mode density operator ρ is defined on the phase space that is a 2n-dimensional real vector space. The characteristic function is
$$
\chi(\xi)=\operatorname{Tr}[\rho \mathcal{W}(\xi)]
$$
Here,$$\mathcal{W}(\xi)=\exp \left(i \xi^{T} R\right)$$is called Weyl operator. The density operator of any quantum state in Fock space can always be written
in terms of its characteristic function and Weyl operators as follows
$$
\rho=\frac{1}{(2 \pi)^{m}} \int d^{2 m} \xi \chi(J \xi) \mathcal{W}(-J \xi)
$$

**A Gaussian state is defined as such a state that its characteristic**
**function is Gaussian:**
$$
\chi(\xi)=\exp \left[-\frac{1}{4} \xi^{T} \gamma \xi+i d^{T} \xi\right]
$$
Here, $$γ > 0$$ is a real symmetric matrix and $$g ∈ \mathbb{R} ^{2n}$$

As shown below, the
quantum vacuum state, coherent states, squeezed states, and thermal states
are typical Gaussian states

