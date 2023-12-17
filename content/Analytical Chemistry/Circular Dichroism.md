---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Circular Dichroism]]
--- 

- What led me here: [[Absorption Spectroscopy]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

# Circular Dichroism

Circular Dichroism (CD) is a spectroscopic technique that measures the difference in absorbance of right-handed and left-handed circularly polarized light (rather than the usual absorbance of isotropic light) by a substance.

## Overview

Circular Dichroism is used to investigate the structural characteristics of optically active molecules, particularly biopolymers such as proteins, nucleic acids, and carbohydrates. The technique is sensitive to the secondary structure of proteins and can therefore be used to determine whether a protein is primarily alpha-helical, beta-sheet, or random coil.

## Principle

The principle of circular dichroism is based on the differential absorption of left and right circularly polarized light by a chiral molecule. When a chiral molecule is exposed to circularly polarized light, it absorbs the two components to different extents, resulting in a difference in absorption that can be measured.

## Applications %% fold %% 

Circular Dichroism has a wide range of applications in various fields, including:

- **Biochemistry**: CD is used to study the secondary structure of proteins and to monitor changes in protein conformation.

- **Pharmaceuticals**: CD is used to determine the enantiomeric purity of a drug and to study the interaction of drugs with biomolecules.

- **Material Science**: CD is used to study the optical properties of various materials, including liquid crystals and polymers.

## References

- Kelly, S. M., Jess, T. J., & Price, N. C. (2005). How to study proteins by circular dichroism. *Biochimica et Biophysica Acta (BBA) - Proteins and Proteomics*, 1751(2), 119-139.
- Greenfield, N. J. (2006). Using circular dichroism spectra to estimate protein secondary structure. *Nature protocols*, 1(6), 2876-2890.
- Berova, N., Di Bari, L., & Pescitelli, G. (2007). Application of electronic circular dichroism in configurational and conformational analysis of organic compounds. *Chemical Society Reviews*, 36(6), 914-931.

### Question: Is it possible to simulate CD from MD
Yes, it is possible to simulate Circular Dichroism (CD) spectra from Molecular Dynamics (MD) simulations. This is typically done by calculating the time-dependent changes in the electronic structure of a molecule during the MD simulation, and then using these changes to simulate the CD spectrum.

The process involves several steps:

1. **Molecular Dynamics Simulation**: An MD simulation is performed on the molecule of interest. This generates a trajectory that describes the time-dependent behavior of the molecule.

2. **Electronic Structure Calculations**: For each time step in the MD trajectory, an electronic structure calculation is performed. This can be done using various methods, such as Density Functional Theory (DFT) or Time-Dependent DFT (TD-DFT).

3. **CD Spectrum Simulation**: The results of the electronic structure calculations are then used to simulate the CD spectrum. This involves calculating the difference in absorption of left-handed and right-handed circularly polarized light by the molecule at each time step, and then averaging these differences over the entire MD trajectory.

This approach allows for the simulation of CD spectra that take into account the dynamic behavior of molecules, which can provide more accurate and detailed information than static CD spectra.


In electronic structure calculations, such as Time-Dependent Density Functional Theory (TD-DFT), the specification of left-handed and right-handed circularly polarized light is not typically done directly. Instead, these calculations usually involve the computation of transition dipole moments, which can then be used to calculate the circular dichroism (CD) spectrum.

The CD spectrum is related to the difference in absorption of left-handed and right-handed circularly polarized light. This difference arises from the transition dipole moments for electronic transitions in the molecule. In a chiral molecule, these transition dipole moments can have a non-zero projection along the direction of propagation of the light, leading to a difference in absorption for the two types of circularly polarized light.

To calculate the CD spectrum from TD-DFT calculations, one typically computes the transition dipole moments for all relevant electronic transitions, and then uses these to calculate the rotational strength for each transition. The CD spectrum is then obtained by summing over the rotational strengths for all transitions, weighted by a line shape function.

It's important to note that the specifics of how to perform these calculations can depend on the particular software package being used. Therefore, it's recommended to consult the documentation for the software package for detailed instructions.


The rotational strength, which is a measure of the intensity of a transition in a circular dichroism (CD) spectrum, is calculated from the transition dipole moments. Specifically, it is given by the dot product of the electric transition dipole moment and the magnetic transition dipole moment.

In mathematical terms, the rotational strength R for a transition from state i to state j is given by:

R_ij = μ_ij . m_ij

where μ_ij is the electric transition dipole moment and m_ij is the magnetic transition dipole moment.

In practice, these quantities are usually calculated as part of a quantum chemical calculation, such as a time-dependent density functional theory (TD-DFT) calculation. Most quantum chemistry software packages can output these quantities.

For example, in Gaussian, you can request the transition dipole moments by including the "TD=(nstates=N)" keyword in the route section of your input file, where N is the number of excited states you want to calculate. The output file will then include a section that lists the transition dipole moments for each excited state.

Once you have the transition dipole moments, you can calculate the rotational strength for each transition and then use these to simulate the CD spectrum.

If you want to do this for many snapshots from a molecular dynamics simulation, you would need to perform a separate TD-DFT calculation for each snapshot. Then, for each snapshot, you would calculate the rotational strengths and simulate the CD spectrum. Finally, you would average the CD spectra from all snapshots to obtain the final spectrum.

Please note that this is a simplified explanation and the actual calculations can be quite complex, depending on the specifics of your system and the level of theory you are using. It's recommended to consult a textbook or review article on computational spectroscopy for more detailed information.

## References

- Stephens, P. J., Devlin, F. J., Chabalowski, C. F., & Frisch, M. J. (1994). Ab Initio Calculation of Vibrational Absorption and Circular Dichroism Spectra Using Density Functional Force Fields. *The Journal of Physical Chemistry*, 98(45), 11623–11627.
- Autschbach, J. (2009). Understanding the basics and subtleties of calculated chiroptical spectra. *Chirality*, 21(E), E116–E131.
- Berova, N., Di Bari, L., & Pescitelli, G. (2007). Application of electronic circular dichroism in configurational and conformational analysis of organic compounds. *Chemical Society Reviews*, 36(6), 914-931.