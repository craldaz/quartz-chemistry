---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[SOAP]]
--- 

- What led me here: [[Molecular Descriptors]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

The Smooth Overlap of Atomic Positions (SOAP) is a versatile and popular descriptor in the field of machine learning with potential applications in materials science and computational chemistry. SOAP was developed by the research group led by Michele Ceriotti in the Laboratory of Computational Science and Modelling at EPFL in Switzerland.

SOAP is a way to encode the local atomic environment in a mathematical form that can be easily used by machine learning algorithms. The goal is to find a representation that is invariant under permutations of atoms and under rotations and translations, which makes it useful for comparing different structures.

The main idea of SOAP is to construct a local density of each type of atom around a given central atom, then take the "overlap" between these densities to construct the descriptor. This procedure is done for all pairs of atomic species, resulting in a two-dimensional matrix. Each entry in this matrix gives the overlap for a specific pair of atomic species. The descriptor is smooth, meaning small changes in atomic positions or types result in small changes in the descriptor.

The SOAP representation has been found to be particularly useful for constructing accurate interatomic potentials, which can be used to perform molecular dynamics simulations for systems that are too large to be feasibly handled with quantum mechanical calculations. It has also been used to predict a wide variety of material properties based on the atomic-scale structure.

