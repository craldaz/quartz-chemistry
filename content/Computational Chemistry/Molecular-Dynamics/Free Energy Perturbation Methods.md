---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Free Energy Perturbation Methods]]
--- 

- What led me here: [[Molecular Dynamics]]

An Alchemical method

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```
[[Lee-Ping Wang]]
![](https://www.youtube.com/watch?v=bMvzvlqVqzU)

# Free Energy Perturbation in Docking Calculations

Free Energy Perturbation (FEP) is a method used in computational chemistry to estimate the difference in free energy between two states, such as the bound and unbound states of a molecule in docking calculations. This technique is particularly useful in drug discovery and molecular dynamics simulations.

## Overview

FEP is based on statistical mechanics and involves gradually changing a system from an initial state to a final state. The difference in free energy between these two states is calculated as an ensemble average over multiple intermediate states.

In the context of docking calculations, FEP can be used to estimate the binding free energy of a ligand to a protein. This is crucial in drug discovery, as it helps predict the affinity of a potential drug molecule to its target protein.

## Process

1. **Initial and Final States**: The initial state typically represents the unbound state of the ligand, while the final state represents the bound state.

2. **Intermediate States**: The system is gradually transformed from the initial to the final state through a series of intermediate states. This is often done by scaling the potential energy function.

3. **Ensemble Averaging**: The free energy difference between each pair of adjacent states is calculated as an ensemble average over a molecular dynamics simulation. 

4. **Free Energy Difference**: The total free energy difference between the initial and final states is obtained by summing up the free energy differences between all pairs of adjacent states.

## Advantages and Limitations

FEP has the advantage of providing a rigorous and theoretically sound method for calculating free energy differences. It can provide detailed insights into the molecular interactions involved in ligand binding.

However, FEP is computationally intensive, as it requires running molecular dynamics simulations for multiple intermediate states. It also requires careful selection of the transformation pathway and the intermediate states.

## Zwanzig equation
The Zwanzig equation, named after Robert Zwanzig, is a fundamental equation in statistical mechanics that is often used in Free Energy Perturbation (FEP) calculations. It provides a theoretical basis for calculating the difference in free energy between two states.

The Zwanzig equation is expressed as:

ΔF = -kT ln <e^(-ΔU/kT)>_0

where ΔF is the free energy difference between two states, k is the Boltzmann constant, T is the temperature, ΔU is the potential energy difference between the two states, and the brackets < >_0 denote an ensemble average over the initial state.

The Zwanzig equation allows us to calculate the free energy difference between two states by running a simulation in only one of the states (usually the initial state) and taking an ensemble average over the exponential of the negative potential energy difference between the two states.


## Alchemy
The concept of "alchemy" in FEP refers to the idea of transforming one molecule into another in a series of intermediate steps. Each step involves a small change in the potential energy function, such as gradually turning off the electrostatic interaction of one atom while turning on the electrostatic interaction of another atom. This is often referred to as "alchemical" transformation because it's reminiscent of the ancient concept of alchemy, where base metals were thought to be transformed into gold.

In the context of FEP, alchemical transformations are used to calculate the free energy difference between two molecular states, such as the bound and unbound states of a ligand, or two different ligands. This can provide valuable insights into the factors that contribute to molecular binding and can help guide the design of new drugs.


## Setup
In a typical Free Energy Perturbation (FEP) setup, the transformation of one chemical species into another is simulated. This process involves categorizing the atoms in the molecular topology into three groups:

1. **Group (i)**: This group consists of atoms that do not change during the simulation. These atoms typically represent the environment or the parts of the molecule that remain constant during the transformation.

2. **Group (ii)**: This group includes atoms that describe the initial state, often denoted as 'a', of the system. These atoms represent the starting molecule or configuration.

3. **Group (iii)**: This group consists of atoms that correspond to the final state, often denoted as 'b', at the end of the alchemical transformation. These atoms represent the target molecule or configuration.

It's important to note that the atoms representing state 'a' do not interact with those of state 'b' throughout the entire molecular dynamics simulation. This setup, where atoms pertaining to both the initial and the final states of the system are present in the molecular topology file (e.g., the psf file), is referred to as the "dual topology" paradigm.

The system's hybrid Hamiltonian, which is a function of the coupling parameter λ, smoothly connects state 'a' to 'b'. The coupling parameter λ is gradually changed from 0 to 1 during the simulation. When λ=0, the system is entirely in state 'a', and when λ=1, the system is entirely in state 'b'. For intermediate values of λ, the system is in a hybrid state that includes features of both 'a' and 'b'.

The Hamiltonian of the system, H(λ), is typically defined as a linear combination of the Hamiltonians of the initial and final states:

H(λ) = (1-λ)H_a + λH_b

The free energy difference between the initial and final states is then calculated as an ensemble average over multiple intermediate states, using the Zwanzig equation. This allows us to estimate the binding affinity of a ligand to a protein or the relative stability of different molecular configurations.

### Interpretation
when the system is in an intermediate state (0 < λ < 1), the dynamics of the system are governed by a hybrid Hamiltonian that is a mixture of the Hamiltonians of the initial and final states. 

The hybrid Hamiltonian is defined as:

H(λ) = (1-λ)H_a + λH_b

where H_a and H_b are the Hamiltonians of the initial and final states, respectively, and λ is the coupling parameter that smoothly interpolates between these two states. 

When λ=0, the system is entirely in state 'a' and follows the dynamics defined by H_a. When λ=1, the system is entirely in state 'b' and follows the dynamics defined by H_b. For intermediate values of λ, the system follows dynamics that are a blend of those defined by H_a and H_b.

This approach allows the system to transition smoothly from the initial state to the final state, enabling the calculation of the free energy difference between these two states.

## References

- Chipot, C., & Pohorille, A. (2007). Free Energy Calculations. Springer.
- Kollman, P. (1993). Free Energy Calculations: Applications to Chemical and Biochemical Phenomena. Chemical Reviews, 93(7), 2395–2417.
- Jorgensen, W. L. (1986). Quantum and statistical mechanical studies of liquids. 10. Transferable intermolecular potential functions for water, alcohols, and ethers. Application to liquid water. Journal of the American Chemical Society, 108(15), 4769–4776.