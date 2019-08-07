# Teleporting an unknown quantum state via dual classical and Einstein-Podolsky-Rosen channels {{"Bennett1993"|cite}}

An unknown quantum state $$|\phi \rangle$$ can be disassembled into, then later reconstructed from, purely
classical information and purely nonclassical Einstein-Podolsky-Rosen (EPR) correlations. To do
so the sender, “Alice,” and the receiver, “Bob,” must prearrange the sharing of an EPR—correlated
pair of particles. Alice makes a joint measurement on her EPR particle and the unknown quantum
system, and sends Bob the Classical result of this measurement. Knowing this, Bob can convert the
state of his EPR particle into an exact replica of the unknown state $$|\phi \rangle$$ which Alice destroyed.

Here, we show that
EPR correlations can nevertheless assist in the “teleportation” of an intact quantum state from one place to
another, by a sender who knows neither the state to be
teleported nor the location of the intended receiver.
Below, we show how
Alice can divide the full information encoded in $$|\phi \rangle$$ into
two parts, one purely classical and the other purely nonclassical, and send them to Bob through two different
channels.
The nonclassical part is transmitted first. To do so,
two spin$$-\frac{1}{2}$$ particles are prepared in an EPR singlet state
$$
|\Psi_{23}^{(-)}\rangle=\sqrt{\frac{1}{2}}(|\uparrow_2 \rangle|\downarrow_3 \rangle-|\downarrow_2 \rangle|\uparrow_3 \rangle)
$$
The subscripts 2 and 3 label the particles in this EPR
pair. Alice’s original particle, whose unknown state $$|\phi \rangle$$
she seeks to teleport to Bob, will be designated by a
subscript 1 when necessary.

One EPR particle (particle 2) is given to Alice, while the other (particle 3) is given to Bob.

To couple the first particle with the EPR pair, Alice
performs a complete measurement of the von Neumann
type on the joint system consisting of particle 1 and particle 2 (her EPR particle). This measurement is performed
in the Bell operator basis consisting of $$|\Psi_{12}^{(-)}\rangle$$ and
$$
|\Psi_{23}^{(+)}\rangle=\sqrt{\frac{1}{2}}(|\uparrow_2 \rangle|\downarrow_3 \rangle+|\downarrow_2 \rangle|\uparrow_3 \rangle)
$$
$$
|\Phi_{23}^{(\pm)}\rangle=\sqrt{\frac{1}{2}}(|\uparrow_2 \rangle|\uparrow_3 \rangle\pm|\downarrow_2 \rangle|\downarrow_3 \rangle)
$$
It is convenient to write the unknown state of the first particle as 
$$
|\phi_1 \rangle=a|\uparrow_1 \rangle+b|\downarrow_1 \rangle
$$
with $$|a|^2+|b|^2=1$$. The complete state of the three
particles before Alice’s measurement is thus
$$
|\Psi_{123}\rangle=\frac{a}{\sqrt{2}}(|\uparrow_1 \rangle|\uparrow_2 \rangle|\downarrow_3 \rangle-|\uparrow_1 \rangle|\downarrow_2 \rangle|\uparrow_3 \rangle)+\frac{b}{\sqrt{2}}(|\downarrow_1 \rangle|\uparrow_2 \rangle|\downarrow_3 \rangle-|\downarrow_1 \rangle|\downarrow_2 \rangle|\uparrow_3 \rangle)
$$
In this equation, each direct product $$|\phantom{\downarrow}_1 \rangle|\phantom{\downarrow}_2 \rangle$$ can be expressed in terms of the Bell operator basis vectors $$|\Phi_{12}^{(\pm)}\rangle$$
and $$|\Psi_{12}^{(\pm)}\rangle$$, and we obtain
$$
|\Psi_{123}\rangle=\frac{1}{2}[|\Psi_{12}^{(-)}\rangle(-a|\uparrow_3 \rangle-b|\downarrow_3 \rangle)+|\Psi_{12}^{(+)}\rangle(-a|\uparrow_3 \rangle+b|\downarrow_3 \rangle)+|\Phi_{12}^{(-)}\rangle(a|\downarrow_3 \rangle+b|\uparrow_3 \rangle)+|\Phi_{12}^{(+)}\rangle(a|\downarrow_3 \rangle-b|\uparrow_3 \rangle)]
$$
$$
\begin{align}
-|\phi_3 \rangle\equiv&-\begin{pmatrix}
a\\b
\end{pmatrix},&\begin{pmatrix}
-1&0\\0&1
\end{pmatrix}|\phi_3 \rangle,\\
&\begin{pmatrix}
0&1\\1&0
\end{pmatrix}|\phi_3 \rangle,&\begin{pmatrix}
0&-1\\1&0
\end{pmatrix}|\phi_3 \rangle.
\end{align}
$$
An
accurate teleportation can be achieved in all cases by
having Alice tell Bob the classical outcome of her measurement, after which Bob applies the required rotation
to transform the state of his particle into a replica of $$|\phi \rangle$$.






