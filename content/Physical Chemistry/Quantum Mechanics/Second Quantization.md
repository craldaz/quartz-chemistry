---
tags: 🧪
---
# `Title:` [[Second Quantization]]
--- 



$\hat{a}^{\dagger}$ - Creation operator
$\hat{a}$ - Annhillation operator


## Uses 
- Second quantization is a standard language used in quantum chemistry
- Hamiltonian can be represented in second quantization in a "coordinate-free" way
-  We can also represent our slater determinant using creation operators from the vacuum state. 
- We can also represent excited determinants from a reference determinant. 
- CASCI type determinants:
    - Can be made efficiently by taking the product of creation operators in the core, and then creation operators in the active. 
- We can describe the CIS, CISD and even Full CI wave function using creation and annihilation operator


## Anticommutation Relationship
$$[\hat{a}^{\dagger}_p,\hat{a}_q]_+ = \delta_{pq}$$



## Normal Ordering 
- Make sure all the creation operators are on the left of the annihilation operators. 
- Must be relative to a particular reference state. 
	- Vacuum state 
	- Fermi vacuum, etc
	

### Wick's Theorem

Tells us what what you need to do to write an operator in normal form. 

For rotation, a normal ordered product is always enclosed in :, e.g.;

$$: \hat{a} \hat{a}^{\dagger} :$$


We define a contraction:
𝐴̂∙𝐵̂∙=𝐴̂𝐵̂ −:𝐴̂𝐵̂ :


Consider all tuples of contractions, then use the rules to determine what the values are 



https://physics.stackexchange.com/questions/477450/what-is-wicks-theorem-and-what-this-is-use-for


### Links: [[Quantum Mechanics]] [[Coupled Cluster Methods]]


