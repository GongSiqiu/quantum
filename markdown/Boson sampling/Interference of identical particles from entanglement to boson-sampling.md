# Interference of identical particles from entanglement to boson-sampling{{"Tichy2014"|cite}} 

This tutorial introduces the physics of many-boson and many-fermion interference required for the description of current experiments and for the understanding of novel approaches to quantum computing.

This tutorial presents an illustrative introduction to the physics of many-boson and many-fermion interference, which supplies the reader the necessary tools to describe photonic entanglement manipulation and novel approaches to optical quantum computing.

## Interference of two particles

### Distinguishable particles: uncorrelated binomial behaviour
Any incoming particle is reflected with probability R and transmitted with probability $$T = 1 -R$$. An *event* with $$s_1$$ and $$s_2$$ particles in the first and second output mode, respectively, occurs with probability $$P_D (s_1 , s_2 )$$. In particular, for a balanced setup, $$T = R = 1/2$$, the distribution of distinguishable particles in the output modes follows a binomial, and 
$$
P_D (2, 0) = \frac{1}{4} , P_D (1, 1) = \frac{1}{2} , P_D (0, 2) = \frac{1}{4}
$$

### Identical particles: correlation without interaction

The creation operator of a particle in input mode $$j$$ is denoted by $$\hat{a}^\dag_ j$$ , such that the initial state reads
$$
|\chi_{\text{ini}}^{(2)}\rangle =\hat{a}_1^\dag\hat{a}_2^\dag|\text{vac}\rangle
$$
where $$|vac\rangle $$denotes the vacuum state. Throughout this tutorial,the letter χ denotes Fock-states, i.e. $$|\chi = |n_1 , n_2 , \cdots\rangle _{1,2,\cdots}$$is interpreted as mode occupation $$n_1 , n_2$$ , etc. The letters $$\psi$$and $$\phi$$ are reserved for qudits controlled by observing parties; $$|\phi\rangle= |\phi_1 , \phi_2 ,\cdots\rangle $$then denotes the state in which $$|\phi_1\rangle$$is observed by the first party, $$|\phi_1\rangle$$by the second, and so on.