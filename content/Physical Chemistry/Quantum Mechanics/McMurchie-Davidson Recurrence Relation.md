---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[McMurchie-Davidson Recurrence Relation]]
--- 

- What led me here: [[Hamiltonian]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

The McMurchie-Davidson Recurrence Relation is a technique used in quantum chemistry for the efficient evaluation of integrals involving Gaussian Type Orbitals (GTOs) and Hermite Gaussians. In many quantum chemistry calculations, such as the evaluation of molecular integrals in ab initio and density functional theory methods, the overlap, kinetic, and potential energy integrals between atomic orbitals need to be determined. Since GTOs are commonly used as basis functions in these calculations, an efficient way to evaluate these integrals is crucial.

The McMurchie-Davidson recurrence relation is a method for evaluating these integrals based on the properties of Hermite Gaussians. Hermite Gaussians are the product of GTOs and Hermite polynomials. The use of Hermite Gaussians simplifies the evaluation of the integrals by taking advantage of the recurrence properties of Hermite polynomials.

The McMurchi-Davidson recurrence relation is derived by applying the product rule of differentiation and the Gaussian product theorem to the integrals. By expressing the integrals in terms of Hermite Gaussians, the problem is reduced to a set of simple one-dimensional integrals that can be efficiently computed using recurrence relations.

The McMurchi-Davidson recurrence relation can be summarized as follows:

1. Express the molecular integrals as integrals of Hermite Gaussians.
2. Use the Gaussian product theorem to combine Gaussian functions.
3. Apply the product rule of differentiation to simplify the integrals.
4. Use the recurrence properties of Hermite polynomials to compute the final values of the integrals.

This method significantly reduces the computational cost of evaluating molecular integrals, making it an essential tool in modern quantum chemistry calculations.