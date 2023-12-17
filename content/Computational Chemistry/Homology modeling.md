---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` 
--- 

- What led me here: [[In Silico Drug Discovery]]

Inlinks
## Homology Modeling in Computational Drug Design

**Homology modeling**, also known as comparative modeling, is a computational method used in structural biology and drug design to predict the three-dimensional structure of a protein based on the known structure of a related protein, the "template". This method is widely used due to the fact that determining a protein's structure experimentally can be time-consuming and costly, while the number of known sequences vastly outnumbers the number of experimentally determined structures.

Homology modeling is based on the principle that protein structure is more conserved than protein sequence. Thus, proteins with similar sequences are likely to have similar three-dimensional structures. It provides valuable structural information which can be used for rational drug design, understanding protein function, and protein engineering.

The process of homology modeling generally involves the following steps:
1. **Template identification and alignment**: A template protein with a known structure and similar sequence to the target protein is identified using database search methods like BLAST. The sequence of the target protein is then aligned with that of the template.
2. **Model Building**: The 3D structure of the target protein is built based on the alignment and the template structure. This is done by constructing the main chain, positioning the side chains, and adding any regions not present in the template.
3. **Model Refinement**: The initial model often contains some errors. It is therefore refined to improve the geometry and fit to the experimental data. This can be achieved through energy minimization and molecular dynamics simulations.
4. **Model Validation**: The quality of the model is evaluated using various statistical and visual analysis methods. 

While homology modeling can provide valuable insights, its limitations should also be noted. The method relies heavily on the quality of the template and sequence alignment, and it is less effective when the sequence identity between the target and the template is below 30%. It is also less effective at predicting the structure of flexible regions that are not well conserved in the template.

**See also**
- [Protein structure](https://en.wikipedia.org/wiki/Protein_structure)
- [Drug design](https://en.wikipedia.org/wiki/Drug_design)
- [Protein–protein interaction prediction](https://en.wikipedia.org/wiki/Protein%E2%80%93protein_interaction_prediction)
- [Molecular modelling](https://en.wikipedia.org/wiki/Molecular_modelling)

**References**
1. Krieger E, Vriend G. Homology modeling. Methods Biochem Anal. 2002;44:509-23. doi: 10.1002/0471200683.ch20.
2. Schwede T. Protein modeling: what happened to the “protein structure gap”? Structure. 2013;21(9):1531-1540. doi:10.1016/j.str.2013.08.007.

This page was last edited on 27 July 2023, at 17:30 (UTC).
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```