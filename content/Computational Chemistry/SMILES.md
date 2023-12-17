---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[SMILES]]
--- 

- What led me here: [[Molecular Representations]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

**SMILES (Simplified Molecular Input Line Entry System)**

SMILES is a notation system that allows for the representation of molecular structure using ASCII strings. It was developed to provide an easily interpretable and transferable way to describe the structural format of chemical species.

### Overview

SMILES represents the structure of a chemical species by encoding the atoms, bonds, and connectivity in a one-dimensional string of characters. Various forms of SMILES exist, including canonical SMILES, which provides a unique representation for each structure.

### Structure

A SMILES string consists of several elements:

- **Atoms**: Represented by their elemental symbols (e.g., 'C' for carbon, 'O' for oxygen).
- **Bonds**: Represented by characters like single (`-`), double (`=`), and triple (`#`) bonds.
- **Branching**: Parentheses `(` `)` are used to show branching in the molecule.
- **Rings**: Numerical digits are used to denote ring closures.
- **Chirality**: '@' symbols represent the stereochemistry.

### Examples

- **Water**: `O`
- **Ethanol**: `CCO`
- **Caffeine**: `CN1C=NC2=C1C(=O)N(C(=O)N2C)C`

### Variations and Extensions

- **InChI**: A standardized format that builds upon the concepts in SMILES.
- **SMARTS**: An extension to SMILES, providing a language for substructure searching.

### Applications

- **Database Searching**: Used in various chemical databases for efficient searching and retrieval of chemical structures.
- **Chemoinformatics**: Employed in computational methods for virtual screening, quantitative structure-activity relationships (QSAR), and other modeling techniques.

### Limitations

- **Ambiguity**: Non-canonical SMILES can lead to different strings representing the same compound.
- **Lack of Information**: Standard SMILES doesn't contain information about isotopes, charge states, or specific tautomeric forms.

### See Also

- [InChI](link)
- [Chemical File Format](link)
- [Chemoinformatics](link)

### References

- Weininger, D. "SMILES, a Chemical Language and Information System. 1