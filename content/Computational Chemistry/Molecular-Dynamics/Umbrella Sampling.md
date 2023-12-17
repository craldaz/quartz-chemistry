---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[personal/Topics/Chemistry/Molecular-Dynamics/Umbrella Sampling]]
--- 

- What led me here: [[Molecular Dynamics]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

# Umbrella Sampling

Umbrella Sampling is a method used in computational chemistry to improve the sampling efficiency of molecular dynamics simulations, especially for systems with high energy barriers. It was first introduced by Torrie and Valleau in 1977.

## Overview

Umbrella Sampling is a type of biased sampling method that uses a biasing potential to enhance the sampling of rare events or regions of phase space that are separated by high energy barriers. The biasing potential, often referred to as the "umbrella potential", is designed to flatten the free energy landscape, hence the name "Umbrella Sampling".

## Potential of Mean Force

The main output of Umbrella Sampling is the Potential of Mean Force (PMF), which is a one-dimensional projection of the multidimensional free energy landscape onto a reaction coordinate. The PMF provides valuable insights into the thermodynamics and kinetics of molecular processes, such as protein folding, ligand binding, and chemical reactions.

The PMF, W(x), is related to the probability density, P(x), along the reaction coordinate, x, by the following equation:

W(x) = -kT ln P(x)

where k is the Boltzmann constant and T is the temperature.

## Procedure

1. **Selection of Reaction Coordinate**: The first step in Umbrella Sampling is to choose a suitable reaction coordinate that describes the process of interest.

2. **Application of Umbrella Potential**: An umbrella potential is applied along the reaction coordinate to enhance the sampling of different regions of phase space.

3. **Running of Simulations**: Multiple simulations are run with different values of the reaction coordinate, each under the influence of a different umbrella potential.

4. **Unbiasing of Data**: The data from the different simulations are combined and corrected for the bias introduced by the umbrella potentials. This is often done using the Weighted Histogram Analysis Method (WHAM).

5. **Calculation of PMF**: The PMF is calculated from the unbiasing probability density along the reaction coordinate.

## Applications

Umbrella Sampling has been widely used in various fields of chemistry and biology, including drug discovery, protein engineering, and materials science. It has been used to study a wide range of molecular processes, such as protein-ligand interactions, protein folding, and ion transport through membranes.

## References

- Torrie, G. M., & Valleau, J. P. (1977). Nonphysical sampling distributions in Monte Carlo free-energy estimation: Umbrella sampling. Journal of Computational Physics, 23(2), 187-199.
- Kumar, S., Rosenberg, J. M., Bouzida, D., Swendsen, R. H., & Kollman, P. A. (1992). The weighted histogram analysis method for free-energy calculations on biomolecules. I. The method. Journal of Computational Chemistry, 13(8), 1011-1021.