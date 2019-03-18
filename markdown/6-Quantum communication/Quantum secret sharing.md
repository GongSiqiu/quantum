# Quantum secret sharing {{"Hillery1999"|cite}}

Secret sharing is a procedure for splitting a message into several parts so that no subset of parts is sufficient
to read the message, but the entire set is. We show how this procedure can be implemented using Greenberger-
Horne-Zeilinger (GHZ) states. In the quantum case the presence of an eavesdropper will introduce errors so
that his presence can be detected. We also show how GHZ states can be used to split quantum information into
two parts so that both parts are necessary to reconstruct the original qubit.

## INTRODUCTION

Secret sharing can be used, for example, to guarantee that no single person can open a vault, has access to an
industrial secret, or can launch a missile with a nuclear warhead, but two together can. This means that for security to be
breached, two people must act in concert, thereby making it
more difficult for any single person who wants to gain illegal
access to the secret information; he must convince the other
party to go along and he risks discovery in the process.

From Alice's original message, she creates two coded messages, one of which
is sent to Bob and the other to Charlie. Each of the encrypted
messages contains no information about her original message, but together they contain the complete message.
(XOR can do this)

We would like to show that it is possible to combine
quantum cryptography with secret sharing in a way that will
allow one to determine whether an eavesdropper has been
active during the secret sharing protocol.

The method for splitting a message into two parts that we
present here uses maximally entangled three-particle states,
or Greenberger-Horne-Zeilinger (GHZ) states.

## GHZ STATES AND SECRET SHARING
Let us suppose that Alice, Bob, and Charlie each have one
particle from a GHZ triplet that is in the state
$$
|\Psi \rangle=\frac{1}{\sqrt{2}}(|000 \rangle+|111 \rangle)
$$
They each choose at random whether to measure their particle in the x or y direction. They then announce publicly in
which direction they have made a measurement, but not the
results of their measurements. Half the time, Bob and Charlie, by combining the results of their measurements, can determine what the result of Alice’s measurement was. This
allows Alice to establish a joint key with Bob and Charlie,
which she can then use to send her message.

$$
|+x \rangle=\frac{1}{\sqrt{2}}(|0 \rangle+|1 \rangle), \quad|+y \rangle=\frac{1}{\sqrt{2}}(|0 \rangle+i|1 \rangle),
$$
$$
|-x \rangle=\frac{1}{\sqrt{2}}(|0 \rangle-|1 \rangle), \quad|-y \rangle=\frac{1}{\sqrt{2}}(|0 \rangle-i|1 \rangle).
$$
$$
|0 \rangle=\frac{1}{\sqrt{2}}(|+x \rangle+|-x \rangle), \quad |1 \rangle=\frac{1}{\sqrt{2}}(|+x \rangle-|-x \rangle),
$$
$$
|\Psi \rangle=\frac{1}{2}[(|+x \rangle_a|+x \rangle_b+|-x \rangle_a|-x \rangle_b)|+x \rangle_c+(|+x \rangle_a|-x \rangle_b+|-x \rangle_a|+x \rangle_b)|-x \rangle_c]
$$
<table width="390.73" border="0" cellpadding="0" cellspacing="0" style='width:232.50pt;border-collapse:collapse;table-layout:fixed;'>
   <col width="103.35" style='mso-width-source:userset;mso-width-alt:3498;'/>
   <col width="71.84" span="4" style='width:42.75pt;'/>
   <tr height="50.42" style='height:30.00pt;mso-height-source:userset;mso-height-alt:600;'>
    <td class="xl65" height="50.42" width="103.35" style='height:30.00pt;width:61.50pt;' x:str><span style='mso-spacerun:yes;'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>Alice<br/>Bob</td>
    <td class="xl66" width="71.84" style='width:42.75pt;' x:str>+x</td>
    <td class="xl66" width="71.84" style='width:42.75pt;' x:str>-x</td>
    <td class="xl66" width="71.84" style='width:42.75pt;' x:str>+y</td>
    <td class="xl66" width="71.84" style='width:42.75pt;' x:str>-y</td>
   </tr>
   <tr height="20.00" style='height:11.90pt;'>
    <td class="xl66" height="20.00" style='height:11.90pt;' x:str>+x</td>
    <td class="xl66" x:str>+x</td>
    <td class="xl66" x:str>-x</td>
    <td class="xl66" x:str>-y</td>
    <td class="xl66" x:str>+y</td>
   </tr>
   <tr height="20.00" style='height:11.90pt;'>
    <td class="xl66" height="20.00" style='height:11.90pt;' x:str>-x</td>
    <td class="xl66" x:str>-x</td>
    <td class="xl66" x:str>+x</td>
    <td class="xl66" x:str>+y</td>
    <td class="xl66" x:str>-y</td>
   </tr>
   <tr height="20.00" style='height:11.90pt;'>
    <td class="xl66" height="20.00" style='height:11.90pt;' x:str>+y</td>
    <td class="xl66" x:str>-y</td>
    <td class="xl66" x:str>+y</td>
    <td class="xl66" x:str>+x</td>
    <td class="xl66" x:str>-x</td>
   </tr>
   <tr height="20.00" style='height:11.90pt;'>
    <td class="xl66" height="20.00" style='height:11.90pt;' x:str>-y</td>
    <td class="xl66" x:str>+y</td>
    <td class="xl66" x:str>-y</td>
    <td class="xl66" x:str>-x</td>
    <td class="xl66" x:str>+x</td>
   </tr>
   <![if supportMisalignedColumns]>
    <tr width="0" style='display:none;'>
     <td width="103" style='width:62;'></td>
    </tr>
   <![endif]>
  </table>


From the table it is clear that if Charlie
knows what measurements Alice and Bob made (that is, x or
y), he can determine whether their results are the same or
opposite and also that he will gain no knowledge of what
their results actually are. Similarly, Bob will not be able to
determine what Alices’s result is without Charlie’s assistance
because he does not know if his result is the same as Alice’s
or the opposite of hers.

With each party choosing to make x or y measurements at
random, only half of the GHZ triplets will give useful results. From the table we can know that if the basis used by Alice and Bob is certain, Charlie can get useful information only by using corresponding basis. 

We assume
that there is an eavesdropper Eve (who could also be either
Bob or Charlie). Her problem is that she does not know what bases have been or
will be used to measure the particles. If she measures them
herself and chooses the wrong bases, she will introduce errors that Alice, Bob, and Charlie will be able to detect by
publicly comparing a subset of their measurements.

In order to show this for a large class of measurements, let
us assume that Eve has been able to entangle an ancilla with
the three-particle state that Alice, Bob, and Charlie are using.
At some later time she can measure the ancilla to gain infor-
mation about the measurement results of Alice, Bob, and
Charlie. The state describing the state of the three particles
and the ancilla is
$$
|\Psi \rangle=\sum^1_{j,k,n=0}|jkn \rangle_3|R_{jkn} \rangle_\xi
$$
where $$|jkn \rangle_3$$ is a state of the three particles and $$|R_{jkn} \rangle_\xi$$ is an
unnormalized ancilla state. What we wish to show is that if
this entanglement introduces no errors into the secret sharing
procedure, then $$|\Psi \rangle$$ must be a product of a GHZ triplet and
the ancilla. This implies that Eve will gain no information
about measurements on the triplet from observing the ancilla or, conversely, if Eve is to gain information about Alice’s
bit, she must invariably introduce errors.

(It is demonstrated by supposing the basis that Alice, Bob, and Charlie used. 
1. All measure
their particles in the x basis
2. Alice measures her particle in the x
basis and Bob and Charlie measure theirs in the y basis.
3. Alice measures her particle in the y direction, Bob measures his in the x direction, and Charlie measures his in
the y direction.
)

Finally, let us conclude this section with a discussion of
the resources necessary to implement quantum secret sharing
protocols. In order to send a shared key containing N bits it is
necessary to use, on average, 2N GHZ triplets. If we instead
use standard quantum cryptography and the classical secret
sharing protocol, then either 4N entangled pairs, using the
Ekert procedure , or 4N particles, using the BB84 procedure, are required. In all cases, the number of particles
sent from Alice to Bob and Charlie is 4N. In the GHZ
scheme, once the key has been established, Alice needs to
send N classical bits in order to transmit the message. These
bits can be sent to either Bob or Charlie using a public channel. In the hybrid quantum-classical scheme Alice must send
2N classical bits once keys with Bob and Charlie have been
established: N bits to send the random string to Charlie and
another N bits to send to Bob the string resulting from the
bitwise XOR of the message and the random string. In general, the more parts into which the secret is split, the greater
the difference between the number of classical bits that must
be sent in the hybrid scheme and in the entangled-state
scheme ($$MN$$ versus $$N$$ for a secret split into $$M$$ parts). We see
that entanglement is able to act as a substitute for transmitted
random bits.

## SPLITTING OF QUANTUM INFORMATION
Now suppose that Alice has a string of qubits she would
like to send to Bob and Charlie in such a way that they must
cooperate in order to extract the quantum information. She
can use shared GHZ triplets $$|000 \rangle_{abc}+|111 \rangle_{abc}$$ and a procedure very similar to quantum teleportation to do this. The
no-cloning theorem implies that only one copy of Alice’s
qubit can be received, so that either Bob or Charlie, but not
both, will possess the final qubit. The procedure we shall
present is symmetric in that either party can end up with the
final qubit, but information from the other party is required
before this can happen. Security could be enforced by requiring that Bob and Charlie meet in person to exchange the final
information and put the qubit to its final use.

Alice begins by taking her qubit, which is in the state
$$\alpha|0 \rangle_A +\beta|1 \rangle_A$$, combining it with her GHZ particle, and
measuring the pair in the Bell basis.

Bob measure his particle and Alice tell Charlie the result of her measurement. Then Bob get the phase information while Charlie get the amplitude information. With the assistance of Bob, Charlie can reconstruct Alice's state.

## FOUR-PARTICLE GHZ STATE
It is possible to generalize this procedure to split information among more than two people. Let us look specifically at
the case of three. Alice starts with a four-particle GHZ state
$$
|\Psi \rangle_4=\frac{1}{\sqrt{2}}(|0000 \rangle+|1111 \rangle)
$$
and keeps one particle for herself and gives one particle each
to Bob, Charlie, and Diana. Her object is to generate a shared
key bit that can only be figured out by Bob, Charlie, and
Diana if they cooperate.
A method of accomplishing this can be found by expressing the state $$|\Psi \rangle_4$$ in different combinations of x and y bases.

Each of the four parties performs a measurement on their particle in either the x or y basis. They then
communicate their choice of basis to Alice (classically), who
decides if the overall basis choice is a usable one, and she
then communicates all four basis choices to each of the other
three parties. Using this information and the results of their
measurements, they can, if they act in concert, determine the
result of Alice’s measurement. This means that Alice, on the
one hand, and Bob, Charlie, and Diana, on the other, will
have, on repeating this process, a shared key.




