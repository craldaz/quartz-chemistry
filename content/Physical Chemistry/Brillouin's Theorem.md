---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Brillouin's Theorem]]
--- 

- What led me here: [[Quantum Mechanics]] [[Hartree Fock Mean Field]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

---

Brillouin's theorem is a fundamental result in quantum chemistry and many-body theory, related to Hartree-Fock (HF) theory.

## Theorem

The theorem states that, for a given HF determinant, any singly excited determinant will yield zero upon integration with the exact wave function, assuming the exact wave function can be written as a power series in the electronic coordinates. This is often expressed as:

`<Ψ(0)|H|Ψ(1)> = 0`

Where Ψ(0) is the reference HF determinant, H is the Hamiltonian operator, and Ψ(1) is any singly excited determinant.

## Relation to Hartree-Fock Theory

Hartree-Fock theory seeks an approximate solution to the Schrödinger equation by assuming a wave function that is a single Slater determinant of spin-orbitals. It forms the basis of post-HF methods such as Coupled Cluster and Configuration Interaction.

In the context of HF theory, Brillouin's theorem indicates that the HF method has already included all single excitations. Any further single excitations will not improve the HF wave function since they're orthogonal to the HF determinant.

## Configuration Interaction Singles (CIS) and Brillouin's Theorem

Configuration Interaction Singles (CIS) is a method that includes all single excitations from a reference determinant, typically the HF determinant. It's often used to calculate excited state energies.

According to Brillouin's theorem, the CIS wave function does not couple to the HF ground state wave function. This means that, when calculating properties, there's no mixing between the ground and excited states due to single excitations.

## Implications

Brillouin's theorem is a key reason why methods that include single excitations on top of the HF reference, such as CIS, do not improve the ground state energy. To obtain a better estimate of the ground state energy, one must include at least double excitations, as methods like Coupled Cluster and Møller-Plesset perturbation theory do.

---

Remember that this is a simplified explanation of Brillouin's theorem and its implications. For a thorough understanding, studying more in-depth quantum chemistry literature is recommended.