---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Boys Function]]
--- 

- What led me here: 

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

Yes, the Boys Function is an additional approach that simplifies the computation of molecular integrals involving Gaussian Type Orbitals (GTOs). It is named after Sidney J. Boys, who introduced this concept in the context of quantum chemistry calculations. The Boys Function deals with the computation of the angular momentum part of the molecular integrals.

Boys Function, denoted as Fm(t), is defined as:

Fm(t) = ∫(0 to 1) exp(-tx²) x^(2m) dx

where m is a non-negative integer and t is a non-negative real number.

In the context of molecular integrals, the Boys Function can be used to evaluate overlap, kinetic, and potential energy integrals involving Gaussian Type Orbitals. The main advantage of the Boys Function is that it allows for the separation of angular and radial parts of the integrals, which greatly simplifies the calculations.

The Boys Function can be evaluated numerically, but there are also various analytical approximations and recursion relations that can be used to compute its values efficiently. One such relation is the downward recurrence relation:

Fm-1(t) = (1/(2m)) * dFm(t)/dt + (2m - 1) * Fm(t) / (2t)

Using the Boys Function in conjunction with the McMurchie-Davidson recurrence relation allows for efficient computation of molecular integrals involving Gaussian Type Orbitals in quantum chemistry calculations. This approach reduces the computational complexity and improves the performance of ab initio electronic structure methods, such as Hartree-Fock and post-Hartree-Fock methods (e.g., Configuration Interaction, Coupled Cluster, and Møller-Plesset perturbation theory).