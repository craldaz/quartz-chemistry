---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[MB-Pol]]
--- 

- What led me here: [[Ab Initio Methods]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```
https://paesanigroup.ucsd.edu/software/mbx.html

[[Vinicius]]

The development of MB-pol started with a detailed analysis of the two- and three-body water interactions evaluated at the CCSD(T) level to quantitatively assess the accuracy of current force fields, DFT models, and ab initio based interaction potentials that are commonly used in molecular simulations [1]. On the basis of this analysis and the results obtained with the HBB2-pol potential [2], the full-dimensional MB-pol potential was developed entirely from "first principles" building upon the many-body expansion of the interaction energy between water molecules [3-5]. 

MB-pol explicitly treats the one-body (intramolecular distortion energy) term and the short-ranged two- and three-body terms. MB-pol can thus be viewed as a classical polarizable potential supplemented by short-range two- and three-body terms that effectively represent quantum-mechanical interactions arising from the overlap of the monomer electron densities. Specifically, at all separations, the total MB-pol two-body term includes (damped) dispersion forces derived from ab initio computed asymptotic expansions of the dispersion energy along with electrostatic contributions due to the interactions between the molecular permanent and induced moments. At short-range, this two-body term is supplemented by a 4th-degree permutationally invariant polynomial that smoothly switches to zero as the oxygen-oxygen separation in the dimer approaches 6.5 Å. Similarly, the MB-pol three-body term includes a three-body polarization term at all separations, which is supplemented by a short-range 4th-degree permutationally invariant polynomial that effectively corrects for the deficiencies of a purely classical representation of the three-body interactions in regions where the electron densities of the three monomers overlap. This short-range three-body contribution is smoothly switched off once the oxygen-oxygen separation between any water molecule and the other two water molecules of a trimer reaches a value of 4.5 Å. In MB-pol, all induced interactions are described through many-body polarization. MB-pol thus contains many-body effects at all monomer separations as well as at all orders, in an explicit way up to the third order and in a mean-field fashion at all higher orders.