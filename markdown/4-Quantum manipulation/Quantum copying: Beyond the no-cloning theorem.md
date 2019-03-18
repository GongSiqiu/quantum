# Quantum copying: Beyond the no-cloning theorem{{"Bu_ek_1996"|cite}}

We analyze the possibility of copying (that is, cloning) arbitrary states of a quantum-mechanical spin-1/2
system.

## INTRODUCTION

The ideal copying process is described by the transformation

$$
|s\rangle_a|Q\rangle_x\rightarrow|s\rangle_a|s\rangle_b|\tilde{Q}\rangle_x\tag{1.1}
$$

where $$|s\rangle_a $$ is the in state of the original mode and $$|Q\rangle_x$$ is the
in state of the copying device.

It have been shown that if a particle in an
arbitrary mixed state is sent into a device and two particles
emerge, it is impossible for the two reduced density matrices
of the two-particle state to be identical to the input density
matrix. Nevertheless, it is still an open question how well
one can copy quantum states, i.e., when ideal copies are not
available how close the copy state (out state in the mode b)
can be to the original state (i.e., $$|s \rangle_a$$ ). The other question to
answer is what happens to the original state $$|s \rangle_a$$ after the
copying.

With the advent of
quantum communication, e.g., quantum cryptography, and
quantum computing, understanding the limits of the manipu-
lations we can perform on quantum information becomes
important.

## WOOTTERS-ZUREK QUANTUM-COPYING MACHINE AND NONCLONING THEOREM
In their paper Wootters and Zurek analyzed the copying process defined by the transformation relation on basis
vectors $$|0\rangle_a$$ and $$|1\rangle_a$$ :
$$
|0\rangle_a|Q\rangle_x\rightarrow|0\rangle_a|0\rangle_b|Q_0\rangle_x
$$

$$
|1\rangle_a|Q\rangle_x\rightarrow|1\rangle_a|1\rangle_b|Q_1\rangle_x
$$



we can assume
that
$$
\sideset{_x}{_x} {\langle Q|Q\rangle}=\sideset{_x}{_x} {\langle Q_0|Q_0\rangle}=\sideset{_x}{_x} {\langle Q_1|Q_1\rangle}=1
$$
The Wootters-Zurek (WZ) quantum-copying machine
(QCM) is defined in such a way that the basis vectors $$|0\rangle_a$$
and $$|1\rangle_a$$ are copied (that is, cloned) ideally, that is, for these
states the relation (1.1) is fulfilled.

The Hilbert-Schmidt norm of an operator Â is given by
$$
\|\hat{A}\|_2=[\text{Tr}(\hat{A}^\dagger\hat{A})]^{1/2}
$$
Our distance between the density matrices $$\hat{\rho}_1$$ and $$\hat{\rho}_2$$ is then
$$
D=(\|\hat{\rho}_1-\hat{\rho}_2\|_2)^2
$$
Other measures of the similarity of two density matrices
have been used. Schumacher  has advocated the use of
fidelity which is defined as
$$
F=\text{Tr}(\hat{\rho}_1^{1/2}\hat{\rho}_2\hat{\rho}_1^{1/2})^{1/2}\tag{2.1}
$$

## INPUT-STATE-INDEPENDENT QUANTUM-COPYING MACHINE
When using this 'universal'
quantum-copying machine (UQCM) superposition states
$$
|s\rangle_a=\alpha|0\rangle_a+\beta|1\rangle_a
$$
 are copied equally well for any value of a in the sense
2
that the distances $$D_a=\text{Tr}[\hat{\rho}_a^{(out)}-\hat{\rho}_a^{(id)}]^2$$
and $$D_{ab}=\text{Tr}[\hat{\rho}_{ab}^{(out)}-\hat{\rho}_{ab}^{(id)}]^2$$ do not depend on the parameter $$\alpha$$.

The most general quantum-copying transformation rules
for pure states on a two-dimensional space can be written as
$$
|0 \rangle_a|Q \rangle_x\rightarrow\sum^1_{k,l=0}|k \rangle_a|l \rangle_b|Q_{kl} \rangle_x,
$$
$$
|1 \rangle_a|Q \rangle_x\rightarrow\sum^1_{m,n=0}|m \rangle_a|n \rangle_b|Q_{mn} \rangle_x,
$$
where the states $$|Q_{mn} \rangle_x$$ are not necessarily orthonormal for all possible values of $$m$$ and $$n$$. The general copying transformation is very complex and it involves many free parameters $$\sideset{x}{x}{ \langle Q_{kl}|Q_{mn}\rangle }$$ which characterize the copying machine.
In what follows we will concentrate our attention on one
particular copying transformation which fulfills our demands
as described above. We propose the transformation
$$
|0 \rangle_a|Q \rangle_x\rightarrow|0 \rangle_a|0 \rangle_b|Q_0 \rangle_x+[|0 \rangle_a|1 \rangle_b+|1 \rangle_a|0 \rangle_b]|Y_0 \rangle_x
$$
$$
|1 \rangle_a|Q \rangle_x\rightarrow|1 \rangle_a|1 \rangle_b|Q_1 \rangle_x+[|0 \rangle_a|1 \rangle_b+|1 \rangle_a|0 \rangle_b]|Y_1 \rangle_x
$$
which is an obvious generalization of the WZ QCM. Due to
the unitarity of the transformation (3.2) the following relations hold:
$$
\sideset{x}{x}{ \langle Q_i|Q_i \rangle}+2\sideset{x}{x}{ \langle Y_i|Y_i \rangle}=1,\quad i=0,1
$$
$$
\sideset{x}{x}{ \langle Y_0|Y_1 \rangle}=\sideset{x}{x}{ \langle Y_1|Y_0 \rangle}=0
$$
There are still many free parameters to specify, therefore we
will further assume that the copying-machine state vectors
$$|Y_i \rangle_x$$ and $$|Q_i \rangle_x$$ are mutually orthogonal:
$$
\sideset{x}{x}{ \langle Q_i|Y_i \rangle}=0, \quad i=0,1
$$
and that
$$
\sideset{x}{x}{ \langle Q_0|Q_1 \rangle}=0
$$
The Hilbert-Schmidt norm
$$
D_a=2 \xi^2(4 \alpha^4-4 \alpha^2+1)+2 \alpha^2(1- \alpha^2)(\eta-1)^2
$$
where we have introduced the notation
$$
\sideset{x}{x}{ \langle Y_0|Y_0 \rangle}=\sideset{x}{x}{ \langle Y_1|Y_1 \rangle}=\xi
$$
$$
\sideset{x}{x}{ \langle Y_0|Q_1 \rangle}=\sideset{x}{x}{ \langle Q_0|Y_1 \rangle}=\sideset{x}{x}{ \langle Q_1|Y_0 \rangle}=\sideset{x}{x}{ \langle Y_1|Q_0 \rangle}=\eta/2
$$
We find that if the parameters j and h are related as
$$
\eta=1-2 \xi
$$
then the norm D a is input-state independent and it takes the
value
$$
D_a=2 \xi^2
$$
$$
\frac{\partial}{\partial \alpha^2}D_{ab}^{(2)}=0
$$
we find $$ \xi =1/6$$. For this value of$$ \xi $$ the norm $$D_{ab}$$is $$\alpha$$independent and its value is equal to 2/9.
### Some properties of the UQCM
1. Any measurement performed on mode $$b$$ affects the
state of mode $$a$$.
2. Once we have found the basis in which both density operators $$\hat{\rho}^{(id)}$$
and $$\hat{\rho}^{(out)}$$
are diagonal we can easily find the
value of the fidelity parameter $$F$$ a as introduced by Schumacher. The fidelity parameter which we are interested in is
given by Eq.(2.1) with $$\hat{\rho}_1=\hat{\rho}_a^{(id)}$$ and $$\hat{\rho}_2=\hat{\rho}_a^{(out)}$$
In our case the fidelity is equal to a constant value $$\sqrt{5/6}$$ for all input
states. We can conclude that the UQCM has that universal
property to be input-state independent, that is, all pure states
are copied equally well.

## MEASUREMENT OF THE ORIGINAL AND THE COPY STATE AT THE OUTPUT OF QCM
In summary the output from the UQCM has the following
property. If any projection is measured in the b mode the
unconditioned a-mode ensemble which results is close to the
ideal output state, i.e., the input state, and can be used to find
the expectation value of any a-mode operator in the ideal
output state. In addition, the b-mode measurement provides
us with information about the input state.

## COPYING STATES IN THE NEIGHBORHOOD OF GIVEN STATE
What we can do
with the output of this copying machine is to use it to calcu-
late the expectation values of any operator which annihilates
this state.

## CONCLUSIONS
A problem with all of these machines is that the copy and
original which appear at the output are entangled. This
means that a measurement of one affects the other. We
found, however, that a nonselective measurement of one of
the output modes will provide information about the input
state and not disturb the reduced density matrix of the other
mode. Therefore the output of these copying machines is
useful.



