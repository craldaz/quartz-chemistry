---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Molecular Descriptors]]
--- 

- What led me here: [[Molecular Representations]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

# Molecular Descriptors

**Molecular descriptors**, in the field of **chemistry** and **chemoinformatics**, are numerical values that characterize the properties of molecules. These descriptors encompass a variety of features such as structural, physicochemical, and quantum mechanical properties, and are extensively used in structure-activity or structure-property relationship studies.

Molecular descriptors are critical in the development and optimization of pharmaceuticals and other chemically-based products, as they facilitate the comparison and prediction of the biological activity, reactivity, or environmental impact of different compounds.

## Types of Molecular Descriptors

Molecular descriptors can be classified into several categories based on the information they encode:

1. **1D descriptors**: These represent global properties of the molecule, such as molecular weight, boiling point, or total surface area.
2. **2D descriptors**: These represent topological or constitutional information, such as the number of rings or bond count in the molecule.
3. **3D descriptors**: These represent three-dimensional spatial configuration of the molecule, including shape and electronic properties. They usually require the knowledge of the 3D structure of the molecule.

## For Energy
See Dscribe github
- Smooth overlap of atomic positions (SOAP)
- Coulomb matrix

1. **Coulomb Matrix (CM)**: The Coulomb matrix is a descriptor used in quantum chemistry to represent the potential energy of interactions in a molecule. Each element of the matrix represents either the Coulombic repulsion between two atoms or the nuclear potential energy of an atom. More specifically, the diagonal elements of the Coulomb matrix are 0.5*Z^2.4, where Z is the atomic number, which can be viewed as an approximation to the atomic self-energy, while the off-diagonal elements are $Z_i*Z_j/|R_i - R_j|$, where Z_i and Z_j are atomic numbers and R_i and R_j are the positions of atoms i and j, representing the Coulombic repulsion between different atoms. One key limitation of the Coulomb matrix is that it is not permutation invariant, meaning that the descriptor changes if the order of the atoms is changed.

2. **Smooth Overlap of Atomic Positions (SOAP)**: SOAP is a method for describing the local environment of atoms in a molecule or a crystal. The idea is to construct a rotationally and translationally invariant descriptor that characterizes the local environment of each atom. This is done by considering the overlap between local "density functions" centered at each atom. The descriptor is smooth, meaning that small changes in the atomic positions lead to small changes in the descriptor, and it captures information about both the types of atoms in the local environment and their positions. SOAP descriptors can be used in a variety of applications, including constructing interatomic potentials and predicting material properties.

Both of these descriptors are used as inputs to machine learning algorithms in materials science and chemistry, allowing these algorithms to "learn" from and make predictions based on the atomic-level structure of molecules and materials.

## See also
* [Quantitative Structure-Activity Relationship (QSAR)](https://en.wikipedia.org/wiki/Quantitative_structure%E2%80%93activity_relationship)
* [Chemoinformatics](https://en.wikipedia.org/wiki/Chemoinformatics)
* [Molecular Modelling](https://en.wikipedia.org/wiki/Molecular_modelling)