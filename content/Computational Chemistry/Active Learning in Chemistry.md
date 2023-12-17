---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Active Learning in Chemistry]]
--- 

- What led me here: [[Machine Learning In Chemistry]] [[Active Learning]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

![](https://youtu.be/QsjyKuazFlA?si=G61jhRBAM0lM9iNn)



## Active Search in Machine Learning (Molecular Optimization)

Active search is a machine learning paradigm that deals with the problem of efficiently finding instances of a particular class within a larger dataset. In the context of molecular optimization, it is used to identify compounds with desirable properties by systematically exploring the vast space of possible molecular structures.

### Overview

Molecular optimization aims to find molecules with specific properties, such as binding affinity, solubility, or stability. Active search combines generative models with an active learning strategy to iteratively refine searches and focus on promising regions of the chemical space.

### Techniques

1. **Generative Models**: Models like Variational Autoencoders (VAEs) or Generative Adversarial Networks (GANs) can generate new molecular structures that are consistent with known examples.

2. **Scoring Function**: Utilized to evaluate the desirability of generated molecules. It can be based on known quantitative structure-property relationships (QSPRs) or learned from data.

3. **Exploration-Exploitation Strategy**: Active search involves a balance between exploring novel regions of the chemical space and exploiting known high-scoring areas. Methods like Upper Confidence Bound (UCB) can be used.

4. **Multi-objective Optimization**: Simultaneously optimizing multiple properties to generate molecules that satisfy complex criteria.

### Applications

- **Drug Discovery**: Finding molecules with optimal binding affinities, toxicity profiles, and other pharmaceutical properties.

- **Material Science**: Designing new materials with specific mechanical, electrical, or optical properties.

### Advantages

- **Efficiency**: Reduces the need for exhaustive searches by intelligently sampling the search space.
- **Flexibility**: Can incorporate various constraints and goals, facilitating the design of highly tailored molecules.

### Challenges and Limitations

- **Complexity**: The high dimensionality of chemical space can make the optimization process challenging.
- **Model Bias**: Dependence on the accuracy of the underlying generative model and scoring function.

### Future Perspectives

Active search in molecular optimization continues to be an active area of research with potential applications in numerous scientific and industrial domains.

### See Also

- [Generative Models](link)
- [Active Learning](link)
- [Drug Discovery](link)

### References

- Gomez-Bombarelli, R.; et al. "Automatic Chemical Design Using a Data-Driven Continuous Representation of Molecules." *ACS Cent. Sci.* 2018, 4, 268–276.

