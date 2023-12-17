---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Using MLFER to optimize Regioselectivity]]
--- 

- What led me here: [[Multiple Linear Regression for Optimizing Homogeneous Catalysts]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

The difference in the transition state energies for the two reaction pathways is often a  useful descriptor in terms of understanding and predicting selectivity. This can be represented as ΔΔE^‡, which is the difference in activation energies between two transition states leading to two different products or regioisomers.

In the context of a multiple linear free-energy relationship, the ΔΔE^‡ could be modeled as a function of different molecular descriptors. Here's an example:

```
ΔΔE^‡ = β0 + β1*σ1 + β2*Es1 + β3*σ2 + β4*Es2 + ... + ε
```

In this equation, σ1 and σ2 could be the Hammett parameters for two different parts of the molecule, Es1 and Es2 could be the Taft parameters for two different parts of the molecule, and ε is the error term. β0, β1, β2, etc., are the regression coefficients that quantify the impact of each descriptor on ΔΔE^‡.

This model provides a way to predict how changes in the molecular structure or the catalyst will influence the difference in transition state energies, and hence, the selectivity of the reaction. By minimizing ΔΔE^‡, you can potentially increase the selectivity towards the desired regioisomer.

As always, predictions made from this model should be experimentally validated to confirm their accuracy, as the model provides correlative relationships, not necessarily causal ones.