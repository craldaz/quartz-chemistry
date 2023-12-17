---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Hartree Fock Mean Field]]
--- 

- What led me here: [[Quantum Mechanics]] [[Approximations in Quantum Chemistry]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

The product of the electrons means mean-field. However, because electrons must be anti-symmetric we must use a determinant. 


# Hartree-Fock Method

## Overview

The Hartree-Fock (HF) method is a computational procedure used in quantum chemistry to approximate the behavior of electrons in a many-electron system. It is named after physicists Douglas Hartree and Vladimir Fock.

## Principle

The Hartree-Fock method is based on the mean-field approximation, where the effect of all the other electrons on a given electron is accounted for by an averaged or "mean" field. This allows the many-electron Schrödinger equation to be reduced to a set of one-electron equations, known as the Hartree-Fock equations.

## Mathematical Formulation

In the Hartree-Fock method, the total wavefunction of the system is approximated as a Slater determinant, which is an antisymmetrized product of single-electron wavefunctions (or "spin orbitals"). The Hartree-Fock equations are then obtained by applying the variational principle to the expectation value of the electronic Hamiltonian.

## Applications

The Hartree-Fock method is widely used in computational chemistry to calculate the properties of molecules and atoms. It serves as the basis for many other electronic structure methods, including post-Hartree-Fock methods (like Møller-Plesset perturbation theory and coupled cluster theory) and density functional theory.

## Limitations

While the Hartree-Fock method is a powerful tool, it has several limitations. It neglects electron correlation, which can lead to significant errors for systems where this effect is important. It also assumes that the system is in its ground state, and does not directly provide information about excited states.

## History

The Hartree-Fock method was developed in the early 20th century as a way to solve the many-electron Schrödinger equation. Despite its limitations, it remains a fundamental method in quantum chemistry and is often the starting point for more accurate calculations.