---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Difference between ECFP and Morgan Fingerprints]]
--- 

- What led me here: [[Extended Connectivity Fingerprint]] [[Morgan Fingerprint]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

The main difference between Extended Connectivity Fingerprint (ECFP) and Morgan fingerprints lies in the way they capture and represent molecular substructures.

ECFP is a circular fingerprinting algorithm that focuses on capturing the local connectivity patterns around each atom in a molecule. It generates a fixed-length bit string by hashing substructural features or "neighborhoods" derived from the molecular graph. ECFP fingerprints are typically used for similarity searching, virtual screening, and other cheminformatics applications. They are robust to small structural changes and computationally efficient.

On the other hand, Morgan fingerprints, also known as circular fingerprints or Morgan algorithm, are based on the concept of "circular atom neighborhoods." Instead of focusing solely on connectivity patterns, Morgan fingerprints consider the presence or absence of substructures within a given radius around each atom. The radius parameter determines the level of detail captured by the fingerprint. Morgan fingerprints are widely used in cheminformatics for similarity searching, machine learning, and other applications.

Here are some key differences between ECFP and Morgan fingerprints:

1. **Representation**: ECFP captures local connectivity patterns, while Morgan fingerprints capture substructures within a specific radius around each atom.

2. **Level of Detail**: ECFP fingerprints can be adjusted in size (number of bits) to control the level of detail captured, whereas Morgan fingerprints' level of detail is determined by the chosen radius parameter.

3. **Robustness**: ECFP fingerprints are relatively robust to small structural changes, making them suitable for comparing structurally similar compounds. Morgan fingerprints, on the other hand, can capture more fine-grained structural details but may be more sensitive to small changes.

4. **Computation**: ECFP fingerprints are computationally efficient to generate and store, while Morgan fingerprints can be more computationally demanding, especially with larger radii.

Both ECFP and Morgan fingerprints have their strengths and are widely used in cheminformatics. The choice between them depends on the specific application, desired level of detail, and computational considerations. Researchers often experiment with both fingerprint types to determine which one performs better for their particular use case.