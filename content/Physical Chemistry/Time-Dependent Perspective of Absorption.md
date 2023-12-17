---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Time-Dependent Perspective of Absorption]]
--- 

- What led me here: [[Quantum Dynamics]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```
====
[[David Tannor]]
[[Fermi’s Golden Rule]]


## Time Dependent Perspective

The absorption spectrum I(ω, T) from a time-dependent perspective can be understood as a measurement of how much a substance absorbs light at different frequencies ω over time T.

In time-dependent quantum mechanics, the absorption spectrum of a system can be calculated from the Fourier transform of the system's correlation function. The correlation function is essentially a measure of how much the system's state at one time is related to its state at another time.

To compute the absorption spectrum, one starts with the system in its ground state, then applies a perturbation (like a light pulse). The system then evolves in time according to the time-dependent Schrödinger equation. The expectation value of the system's dipole moment is then calculated as a function of time. This gives the dipole correlation function, which can be Fourier transformed to give the absorption spectrum I(ω, T).

The resulting absorption spectrum gives the absorption intensity (I) as a function of the light frequency (ω) and time (T). Peaks in the absorption spectrum correspond to energies at which the system can absorb a photon and transition from the ground state to an excited state.

The formal expression in terms of the dipole-dipole correlation function is typically given by:

    I(ω, T) = ∫〈μ(0)·μ(t)〉e^(-iωt) dt

where:

- ∫ denotes the integral over time.
- μ(t) is the dipole moment operator in the Heisenberg picture at time t.
- 〈...〉 denotes the quantum mechanical expectation value.
- e^(-iωt) is the complex exponential function which is introduced for the Fourier transformation.
- ω is the frequency of light.

This provides a way to connect the time-dependent behavior of a quantum system to experimentally observable quantities, like the absorption spectrum.
## From Chat GPT CRA-2023-07-06
David Tannor's work, particularly in quantum mechanics and quantum dynamics, is highly regarded. His reference to two steps in first-order perturbation theory to get back to real numbers can be interpreted in the context of time-dependent perturbation theory.

In time-dependent perturbation theory, the solution process often involves two steps. First, you apply a time-dependent perturbation to a system and allow it to evolve from the initial state according to the time-dependent Schrödinger equation. Second, you calculate the probability amplitude for the system to be found in a different (final) state after some time. This often involves calculating complex quantities, due to the imaginary unit 'i' in the Schrödinger equation.

Let's consider a transition from an initial state |i> to a final state |f> driven by a perturbation. The first order perturbation in the transition amplitude is typically an integral involving the time-evolution of the perturbation and the overlap of the initial and final states, and is generally a complex quantity:

    c_f(t) = - (i/ħ) ∫〈f|H'|i〉e^(iω_if t) dt (from 0 to t)

where:
- c_f(t) is the first order coefficient for the final state
- H' is the perturbation Hamiltonian
- ω_if = (E_i - E_f) / ħ is the frequency associated with the energy difference between the initial and final states

But what we're physically interested in is not the complex transition amplitude, but the transition probability, which is the magnitude squared of the amplitude:

    P_if(t) = |c_f(t)|^2

This squaring operation (step two) brings us back to real numbers, as it involves taking a complex number and multiplying it by its complex conjugate, which always yields a real number.

So, in this context, Tannor's statement could be understood as referring to the two steps of 1) calculating the complex transition amplitude through time-dependent perturbation theory, and then 2) calculating the transition probability, which is a real number, from the amplitude.


In quantum mechanics, the density matrix (also called the density operator) is a way of describing the statistical state of a quantum system. It's especially useful when we are dealing with a mixed state, a statistical mixture of different quantum states. 

For a two-state quantum system, the density matrix ρ is a 2x2 matrix. If we label the two states as |0> and |1>, the density matrix is usually written as follows:

    ρ = [p_00   p_01]
        [p_10   p_11]

where p_00 and p_11 are the probabilities of the system being in states |0> and |1> respectively, and p_01 and p_10 are the coherences, which represent the "interference" between the two states.

In quantum dynamics, it's possible for population (i.e., probability density) to transfer between states |0> and |1>. This might be due to some kind of interaction or perturbation that the system experiences.

The off-diagonal elements p_01 and p_10 play an important role in this transfer. They provide a "pathway" for population transfer between the two states. In a sense, these elements represent the quantum mechanical "overlap" between states |0> and |1>.

The transfer of population from p_00 to p_11 would therefore involve these coherences, as you were told. The precise nature of this transfer would depend on the specifics of the system's Hamiltonian (i.e., the specifics of the energies of the states and the interactions between them).

This kind of dynamics, where population transfers between states through off-diagonal coherences, is a distinctly quantum mechanical phenomenon. It's one of the ways in which quantum systems can behave quite differently from classical one.

## Eric Heller
Eric J. Heller's work on semiclassical methods provides a bridge between the quantum and classical descriptions of dynamical systems, which can be particularly useful in the analysis of molecular dynamics and spectroscopy.

Heller's semiclassical approach involves the use of "wave packets" to describe quantum mechanical systems. Wave packets are localized collections of waves that can exhibit both particle-like and wave-like behavior. This makes them useful for describing quantum systems in a manner that has a more intuitive connection to classical physics.

In Heller's wave packet dynamics, he constructs a wave packet in a manner that it approximately follows classical trajectories. The time evolution of these wave packets are then studied under the influence of the Hamiltonian, giving a semiclassical perspective on the dynamics of the system.

In the context of spectroscopy, and absorption spectroscopy in particular, Heller's semiclassical approach can be employed to calculate the absorption spectrum. The time-dependent perspective of absorption, as we discussed earlier, is an expectation value of the system's dipole moment as a function of time. In Heller's wave packet dynamics, the system is initially prepared in a superposition of states (a wave packet), and the absorption spectrum is calculated from the Fourier transform of the time-dependent dipole moment. This dipole moment is calculated as an expectation value over the wave packet, providing a semiclassical perspective on the absorption process.

This semiclassical approach can be very useful in situations where purely quantum mechanical methods may be too computationally intensive. It provides a method for understanding and calculating the behavior of quantum systems in a manner that has a more direct connection to our classical intuition.