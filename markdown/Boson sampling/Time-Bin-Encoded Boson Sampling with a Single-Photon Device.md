---
typora-root-url: ../../image
---

# Time-Bin-Encoded Boson Sampling {{"He2017"|cite}} 

## Photon source

An intrinsic problem in the SPDC, however,is that the photon pairs are generated probabilistically,
and mixed with double pair emission. To scale up to a larger number of photons and fast sampling rate, a more efficient route is to use single-photon sources that emit one and only one photon each time. Here is quantum dot(QD) micropillar.

## Scheme

 <embed
 src="../image/schemwtimebin.svg" 
 alt="scheme"
 width="750"
 height="350"/>

For each experimental period, M time bins(each loaded with one or zero photon) are injected into a loop by an acousto-optical modulator (AOM) and circulated for N loops. Such a loop-based architecture is equivalent to an M-mode beam splitter network with a depth of N, as illustrated in Fig(b). Here, the polarization degree of freedom acts as the spatial mode in the conventional boson sampling model. The beam splitter operations, denoted by the circles in Fig(b), are effectively realized using a polarization-rotation electro-optic modulator (p-EOM) with dynamically programmable coupling ratio. After the p-EOM, a polarization-dependent asymmetric Mach-Zehnder interferometer delays the vertical polarization for one time-bin length (∼13 ns), regarding to the horizontal polarization, which realizes the displacement operation of the time bins. After N loops of evolution, the M bins are ejected out of the loop by another AOM, and the output distributions are obtained by registering all of the single-photon detectionevents in real time and postprocessing . We calibrate the mode matching of the time-bin loop using Mach-Zehnder interference. The time-bin encoding scheme naturally complements the single-photon pulse train.

## Strength

The loop-based architecture is intrinsically stable, electrically programmable, and resource efficient. For an arbitrary n-boson sampling, this scheme requires only one single-photon emitter, two optical switches, two EOMs, and two fast detectors, whereas the traditional spatial-encoding approach requires $$n-1$$ optical switches, $$ \sim n^4 $$  beam splitters, and $$\sim n^2$$detectors.  Furthermore, it relaxes the overhead of actively demultiplexing a single-photon source or building an array of multiple identical single-photon sources

## limitation

The overall efficiency of the current experiment is
mainly limited by the system efficiency of the single-
photon source (∼24.7%, due to losses in light extraction,cross polarization, optical path transmission, and fiber coupling), transmission of the loop-based interferometer(∼83.4% per loop), and single-photon detection efficiency(∼52%).

## Error

The slight fidelity decrease might be mainly due to the mode mismatching (0.5%) per loop

## Significance

The flexible loop-based architecture in this experiment further allows us to track the dynamical multiphoton evolution in the circuit at intermediate time. This experiment opens a new way to study multiparticle high-dimensional quantum walks with single quantum emitters, and opens up a new avenue to multiphoton quantum computation with single quantum emitters, and brings boson sampling closer to an experimental regime approaching quantum supremacy.



