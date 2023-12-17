---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Andersen Barostat]]
--- 

- What led me here: [[Barostats]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

The Andersen barostat is a method used in molecular dynamics simulations to maintain constant pressure in the system while allowing the volume to fluctuate. It was first introduced by Hans C. Andersen in 1980. The Andersen barostat is based on the idea of stochastically rescaling the volume and positions of the particles in the system, which emulates the effect of collisions with an imaginary piston. The main features and characteristics of the Andersen barostat are as follows:

1. Stochastic approach: Unlike the Berendsen barostat, which weakly couples the system to an external pressure bath and scales the system's volume continuously, the Andersen barostat adjusts the volume of the system stochastically. This means that the volume and positions of the particles are rescaled at random intervals, based on a probability distribution derived from the difference between the current pressure and the target pressure.

2. Monte Carlo moves: In the Andersen barostat, the system's volume is adjusted using Monte Carlo moves. A trial move is proposed by stochastically changing the volume, and the change is accepted or rejected based on the Metropolis-Hastings criterion. This criterion takes into account the difference in potential energy and the change in the volume of the system.

3. Isoenthalpic-isobaric ensemble: The Andersen barostat maintains the system in the constant enthalpy (H), constant pressure (P), and constant number of particles (N) ensemble, also known as the NPH ensemble. This ensemble is appropriate for simulating systems where the energy exchange with the environment is negligible, and the pressure is the controlled variable.

4. Ensemble averages: The stochastic approach used in the Andersen barostat allows it to generate the correct ensemble averages for systems in the NPH ensemble. This is an advantage over the Berendsen barostat, which does not produce accurate ensemble averages due to its weak coupling to the pressure bath.

5. Artifacts: One of the drawbacks of the Andersen barostat is that it can introduce sudden jumps in the system's volume due to its stochastic nature. These jumps can lead to artifacts in the simulation results, especially for systems with highly anisotropic or long-range interactions.

Despite its limitations, the Andersen barostat is widely used in molecular dynamics simulations due to its ability to produce accurate ensemble averages and its relative simplicity compared to more complex barostat algorithms, like the Parrinello-Rahman or Martyna-Tobias-Klein barostats.