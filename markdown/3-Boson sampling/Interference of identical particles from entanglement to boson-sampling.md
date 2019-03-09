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

The creation operator of a particle in input mode $$j$$ is denoted by $$\hat{a}^\dagger_j$$ , such that the initial state reads
$$
|\chi_{\text{ini}}^{(2)}\rangle =\hat{a}_1^\dagger\hat{a}_2^\dagger|\text{vac}\rangle
$$

where $$|\text{vac}\rangle$$ denotes the vacuum state. Throughout this tutorial,the letter $$\chi$$ denotes Fock-states, i.e. $$|\chi\rangle = |n_1 , n_2 , \cdots\rangle _{1,2,\cdots}$$ is interpreted as mode occupation $$n_1 , n_2$$ , etc. The letters $$\psi$$ and $$\phi$$ are reserved for qudits controlled by observing parties; $$|\phi\rangle= |\phi_1 , \phi_2 ,\cdots\rangle$$ then denotes the state in which $$|\phi_1\rangle$$ is observed by the first party, $$|\phi_1\rangle$$ by the second, and so on.

The time-evolution of particle creation operators in the Heisenberg picture reads accordingly
$$
\hat{a}_j^\dagger\to\hat{U}\hat{a}_j^\dagger\hat{U}^{-1}=i\sqrt{R}\hat{b}_j^\dagger+\sqrt{T}\hat{b}_{3-j}^\dagger
$$
the single-particle wavefunction acquires a phase-shift of $$i = e ^{i\pi/2} $$ upon reflection. The single-particle time-evolution can be inserted into the initial state, and, for a balanced beam splitter $$(R = T = 1/2)$$, the final state becomes
$$
|\chi^{(2)}_{fin}\rangle=\frac{1}{2}(\text{i}(\hat{b}_1^\dagger)^2+\text{i}(\hat{b}_2^\dagger)^2-\hat{b}_1^\dagger\hat{b}_2^\dagger+\hat{b}_2^\dagger\hat{b}_1^\dagger)|\text{vac}\rangle
$$
*Fermions* $$(\hat{b}_j^\dagger)^2=0$$ for fermionic creation operators. The final state becomes
$$
|\chi^{(2)}_{fin,F}\rangle=\hat{b}_2^\dagger\hat{b}_1^\dagger|\text{vac}\rangle=|1,1\rangle_{1,2}
$$
from which we immediately read off
$$
P_F (2, 0) = 0, P_F (1, 1) = 1, P_F (0, 2) = 0
$$


The Pauli principle prohibits the double
population of any output mode, which is compatible with
the constructive collective interference that enhances the
probability to find the particles in different modes.

*Bosons* 
$$
P_F (2, 0) = \frac{1}{2}, P_F (1, 1) = 0, P_F (0, 2) = \frac{1}{2}
$$
Bosonic bunching and
the Pauli principle are not the consequence of coherently superimposed many-particle paths, but they are rather kinematic
boundary conditions on the state-space of identical particles.

Collective many-particle interference can only affect
many-particle observables

### Two-particle distinguishability transition

#### Two partially distinguishable bosons

As a realistic
example for such transition, we consider photons and choose
the time of arrival at the beam splitter as the degree of
freedom through which the indistinguishability of the light
quanta may be affected. In quantum optics experiments ,
the relative delay in the arrival time is manipulated by the
spatial displacement of the wave-packets to the beam splitter.

The resulting event probability for partially distinguish-
able particles becomes the average of the probabilities assigned
to bosons and to distinguishable particles, weighted by $$|c_{2,1}|^2
$$and $$|c_{2,2}|^2$$ , respectively: 
$$
P_T(\vec{s}=(s_1,s_2),x)=|c_{2,1}|^2P_B(s_1,s_2)+|c_{2,2}|^2P_D(s_1,s_2)
$$
To model typical experiments with photons , a
Gaussian frequency distribution around a central frequency
$$\omega_0$$ with width $$\Delta \omega$$ is assumed,
$$
|t_j\rangle=\int\mathop{}\!\mathrm{d}\omega\frac{1}{\pi^{1/4}\Delta\omega^{1/2}}e^{-\frac{(\omega-\omega_0)^2}{2\Delta\omega^2}}e^{i\omega t_j}|\omega\rangle
$$
The temporal overlap of two photons then becomes
$$
\begin{align}
\langle t_j|t_k\rangle 
& =\frac{1}{\pi^{1/2}\Delta\omega}\iint\mathop{}\!\mathrm{d}\omega_1\mathop{}\!\mathrm{d}\omega_2 e^{-\frac{(\omega_1-\omega_0)^2+(\omega_2-\omega_0)^2}{2\Delta\omega^2}}e^{i\omega_1 t_j+i\omega_2 t_k}\langle\omega_1|\omega_2\rangle




\\ & =\frac{1}{\pi^{1/2}\Delta\omega}\int\mathop{}\!\mathrm{d}\omega_2 e^{-\frac{(\omega_2-\omega_0)^2}{\Delta\omega^2}}e^{i\omega_2 (t_j+t_k)}
 


\\ & =e^{i(t_k-t_j)\omega_0}e^{-\frac{(t_j-t_k)^2}{4}\Delta\omega^2}
\end{align}
$$

The visibility of the HOM-dip constitutes today the defacto standard for ensuring the indistinguishability of two bosonic particles in the experiment.

By post-selecting events with a well-defined total number
of photons N, i.e. by neglecting all final events in which the
total number of detected photons does not match the desired
N, one can effectively project with high fidelity onto the
component with a total of N light quanta in the initial state.

### Bipartite entanglement generation

#### Generation of classical correlations

the outcomes
of the measurements are determined by the distribution of the
objects among the observers, i.e. before the detection actually
takes place.

#### Quantum correlations via propagation and detection.

$$
|\chi^{2ent}_{fin}\rangle=\frac{1}{2}(\text{i}(\hat{b}_{2,0}^\dagger\hat{b}_{1,1}^\dagger+\hat{b}_{1,0}^\dagger\hat{b}^\dagger_{2,1})+\hat{b}_{2,0}^\dagger\hat{b}_{1,1}^\dagger-\hat{b}_{1,0}^\dagger\hat{b}_{2,1}^\dagger)|\text{vac}\rangle
$$

By post-selecting those events with
exactly one particle per spatial output mode, i.e. coincident
events, we can effectively project the
state onto 
$$
|\chi^{2ent}_{fin}\rangle=\frac{\sqrt{2}}{2}(\hat{b}_{2,0}^\dagger\hat{b}_{1,1}^\dagger-\delta\hat{b}_{1,0}^\dagger\hat{b}_{2,1}^\dagger)|\text{vac}\rangle
$$
where $$\delta = +1$$ for bosons and $$\delta= −1$$ takes into account the
anti-commutation relation of fermionic creation operators.

#### Partial distinguishability and degradation of entanglement.
If the particles prepared in the input
modes do not differ only in the degree of freedom in which
entanglement is to be created, but also in
another physical property, the correlations measured at the
output modes will eventually degrade to purely classical ones.
In practice, this deteriorating degree of freedom is often the
time of arrival.

The
indistinguishability $$|c_{2,1}|^2$$ directly quantifies the many-body
coherences of the emerging state and, thus, the quantum nature
of the induced correlations. Indeed, a quantitative indicator for
entanglement, the concurrence
$$
C=|c_{2,1}|
$$
directly reflects the indistinguishability



Relying on propagation and detection for entanglement
manipulation also leads to natural constraints on operations.
For example, a measurement that fully discriminates all four
Bell states is impossible, which inhibits deterministic
teleportation, for which nonlinear interactions are
necessary.

## Many-particle interference

### Many-particle evolution and transition probabilities

#### Distinguishable particles

$$
P_D(\vec{r},\vec{s};U)=\sum_{\sigma\in S_{\vec{d}(\vec{s})}}\prod^N_{j=1}p_{d_j(\vec{r},\sigma(j))}
$$

#### indistinguishable particles

For indistinguishable
particles, the argument can be repeated. Now, however, the
exchange of two particles in the output modes does not
change the quantum state (up to a global sign change for
fermions), such that all possibilities to distribute the particles
among the output modes contribute coherently to the final
state. As a consequence, many-body amplitudes of the form $$U_{d_1 (\vec{r} ),d_1 (\vec{s} )}U_{d_2 (\vec{r} ),d_2 (\vec{s} )}\cdots U_{d_N (\vec{r} ),d_N (\vec{s} )}$$  need to be summed
$$
P_B(\vec{r},\vec{s};U)=\frac{\prod_js_j!}{\prod_jr_j!}\left|\sum_{\sigma\in S_{\vec{d}(\vec{s})}}\prod^N_{j=1}U_{d_j(\vec{r},\sigma(j))}\right|^2
$$

$$
P_F(\vec{r},\vec{s};U)=\left|\sum_{\sigma\in S_{\vec{d}(\vec{s})}}\mathrm{sgn}(\sigma)\prod^N_{j=1}U_{d_j(\vec{r},\sigma(j))}\right|^2
$$

where $$\mathrm{sgn}(\sigma)$$ takes into account the phase acquired upon
exchange of two fermions in the output modes.

#### Coarse-grained statistical signatures

For Pauli arrangements, the difference between the
average probability for bosons and fermions dies out when
the density of particles N/n is decreased: in the dilute limit
N/n → 0, bunched events with several particles per mode
are a priori very unlikely, and their influence on the statistics vanishes

For fully bunched events for which one mode receives
all particles, $$\vec{s_b} = (0, . . . , 0, N, 0 . . . , 0)$$, we can formulate
an exact relation between the probabilities for distinguishable
particles and bosons
$$
P_B(\vec{r},\vec{s_b};U)=\frac{N!}{\prod_jr_j!}P_D(\vec{r},\vec{s}_b;U)\geqslant P_D(\vec{r},\vec{s_b};U)
$$
On the other hand, if all bosons are prepared in the same
mode, the probabilities for
bosons and distinguishable particles do not differ at all.



#### Determinants, permanents and computational complexity

In order to find a
more compact expression for the probabilities, a characteristic
$$N \times N$$-matrix can be defined as
$$
M_{j,k}=U_{d_j(\vec{r}),d_k(\vec{s})}
$$
i.e. M contains those rows and columns of U that correspond
to (possibly multiply) occupied in- and output modes,
respectively. With M defined as such, we can write
$$
\begin{align}
P_D(\vec{r},\vec{s};U)&=\frac{1}{\prod_{j=1}^ns_j!}\sum_{\sigma\in S(\{1,\dots,N\})}\prod^N_{k=1}|M_{k,\sigma(k)}|^2\\
&=\frac{1}{\prod_{j=1}^ns_j!}\text{perm}(|M|^2)
\end{align}
$$


where the function $$\text{perm} (|M| ^2 ) $$is the permanent of the
matrix $$|M| ^2$$ , for which the absolute-square is taken
component-wise. For bosons, we find
$$
P_B(\vec{r},\vec{s};U)=\frac{1}{\prod_{j=1}^ns_j!}|\text{perm}(M)|^2 \tag{PB}
$$
i.e. the permanent of the complex **matrix** $$M$$ needs to be
computed before taking the absolute-square to obtain the probability. For fermions, the sign-change allows us to identify
the total amplitude as a determinant,
$$
P_F(\vec{r},\vec{s};U)=|\text{det}(M)|^2
$$
The evaluation
of the determinant can be performed in time polynomial in the
matrix size $$N$$.

For distinguishable particles, by sampling over many randomly chosen
permutations $$\sigma$$ , the permanent can be estimated.



#### Boson-sampling

It is tempting to state that quantum mechanics makes it
possible to 'compute the permanent of a complex matrix
with exponential speedup with respect to classical computers'
using bosons that propagate through a multimode setup. However, even though the amplitudes of final
states characterized by $$\vec{s}$$ correspond to the permanent of a
certain matrix $$M$$, these amplitudes are very small, which
makes them difficult to extract. Although it is possible to define
an observable whose expectation value coincides with the permanent, its large variance requires an exponential number
of measurements to extract the permanent experimentally
. This caveat jeopardizes any strategy to directly compute
the permanent via the scattering of bosons, although there are
current attempts in this direction.



#### Can we trust a boson-sampling device?

An alternative approach to certifying boson-sampling
devices is to leave the space of computationally complex
problems: instead of choosing the scattering matrix randomly
according to the unitary Haar-measure (which is a crucial
assumption for the very hardness of the problem ), one
can artificially design test-cases for which pertinent properties
of the resulting probability distribution are obtained efficiently
on a classical computer. In other words, the boson-sampling
device is assessed by a task whose exact or approximate
solution is known beforehand.

One approach is based on processes with well-understood
average behaviour, such as many-particle quantum walks.In other words, although bosonic statistical effects
witness features that go beyond the uncorrelated behaviour
of distinguishable particles, the observation of these effects is
nevertheless insufficient to strictly guarantee a behaviour in accordance to equation (PB).



#### A falsifiable instance of boson-sampling: the Fourier suppression law

The superior computational
complexity of many-boson scattering in comparison to the
analogous problem with fermions is rooted in the absence
of symmetries of the permanent compared to the more
benevolent determinant. 

Our strategy to devise a solvable
instance of boson-sampling therefore relies on imposing
artificial symmetries on the scattering matrix  $$U$$, which then
allows us to exactly compute the permanent of the pertinent
submatrices in a large number of cases.