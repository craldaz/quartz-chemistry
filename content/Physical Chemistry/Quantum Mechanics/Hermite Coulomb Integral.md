---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Hermite Coulomb Integral]]
--- 

- What led me here: [[Hamiltonian]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

The Hermite Coulomb Integral (HCI) is an important component in the computation of electron repulsion integrals (ERIs) in quantum chemistry calculations involving Gaussian Type Orbitals (GTOs). The [[Boys Function]] is used to simplify the calculation of the angular momentum part of the HCI, making it more computationally efficient.

In the context of ERIs, the HCI is defined as:

HCI(a, b, p, q, m) = ∫(0 to 1) exp(-ax²) x^(2a) ∫(0 to 1) exp(-by²) y^(2b) R_pq(x, y) dy dx

where a and b are non-negative integers, p and q are the centers of the Gaussian functions, and R_pq(x, y) is the Coulomb interaction between two Gaussian charge distributions with centers p and q.

To simplify the calculation of the HCI, the Boys Function can be introduced by performing a change of variables and separating the radial and angular components of the integrals:

HCI(a, b, p, q, m) = Fm(t) * A(a, b, p, q)

where Fm(t) is the Boys Function, and A(a, b, p, q) is the angular momentum integral. The Boys Function takes care of the radial part of the HCI, while A(a, b, p, q) handles the angular part.

In this way, the Boys Function helps in reducing the computational complexity of the HCI, which, in turn, simplifies the calculation of electron repulsion integrals involving Gaussian Type Orbitals. This improvement in efficiency is particularly important for ab initio electronic structure methods, such as Hartree-Fock and post-Hartree-Fock methods, where ERIs can be one of the most computationally demanding parts of the calculations.