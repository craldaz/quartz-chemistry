---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Principle Moment of Inertia Plot]]
--- 

- What led me here: [[Cheminformatics]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

### PMI for Molecular Diversity Plot

**Principal Moments of Inertia (PMI)** is a method used to analyze molecular shapes and diversity within a set of compounds. It provides a graphical representation of molecular structures, aiding in the understanding of structure-activity relationships.

#### Overview

PMI involves the calculation of the principal moments of inertia (I1, I2, I3) for a molecule. These values correspond to the three orthogonal axes of a molecule and provide insight into its overall shape.

#### Shape Classification

By plotting the normalized values of the principal moments of inertia, molecules can be categorized into various shape classes:

1. **Spherical**: I1 ≈ I2 ≈ I3
2. **Prolate (Rod-like)**: I1 ≈ I2 < I3
3. **Oblate (Disc-like)**: I1 < I2 ≈ I3

#### Applications

1. **Molecular Diversity Analysis**: PMI plots allow for the visualization and comparison of molecular shapes within a library, highlighting diversity.
2. **Drug Discovery**: Understanding shape diversity is vital in the design of new pharmaceutical compounds.
3. **Material Science**: Shape analysis is used in the design of new materials with specific properties.

#### Plotting the PMI

A PMI plot is typically a 2D or 3D scatter plot, with axes representing the normalized principal moments of inertia. The plot provides a visual representation of the shapes of molecules in the dataset.

#### Advantages and Limitations

- **Advantages**: Simple, effective visualization of molecular shape; useful for comparing large sets of compounds.
- **Limitations**: May oversimplify complex structures; limited to rigid molecules without considering flexibility.

#### Example Software

Several computational chemistry tools can be used to generate PMI plots, such as:

- RDKit
- Open Babel
- Schrödinger Suite

#### See Also

- [Molecular Geometry](https://en.wikipedia.org/wiki/Molecular_geometry)
- [Chemoinformatics](https://en.wikipedia.org/wiki/Chemoinformatics)
- [Molecular Modelling](https://en.wikipedia.org/wiki/Molecular_modelling)

---

The PMI for molecular diversity plot is an elegant and informative method to analyze and visualize molecular shapes. It has found applications in various domains, contributing significantly to the understanding of structure-activity relationships.