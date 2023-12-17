---
tags: 🧪
CssClass:
    - wide
---


# `Title:` [[Ab Initio Multiple Spawning]]
[[Full Multiple Spawning]]

 [[Semi-classical Dynamics]]

---

## Overview

AIMs is an approximation of Full Multiple Spawning that utilizes two approximations: 
1. Independent first generation (IFG)
2. Saddle point approximation

### IFG
The IFG approximation considers all initial TBFs to be uncoupled (so they can be run independentally). 

To each parent is associated a given branch $\beta$. Each parent TBF can have child TBFs (and so on).


There is coupling of TBFs within a branch but not between branches.

$$\Psi(r,R,t) = \sum_{\beta}^{N_{ini}}\Psi_{\beta}(r,R,t)$$
$$=\sum_{\beta}^{N_{ini}}\sum_{\nu}^{\inf}\sum_k^{N_v^{\beta}}C_{k\beta}^{(v)}...$$


For example, the parent TBF in the first branch ($\beta=1$) in state v, would have complex coefficient $C_{11}^v$, and the first child of this tbf on state u would have coefficient $C_{21}^u$


### Saddle point approximation
Some integrals in the Hamiltonian are performed over the nuclear coordinates while containing electronic structure quantities like the elctronic energies or the non-adiabatic couplings. Calculating these integrals would imply knowing these electronic structure quantities over all the configuration space. Which would require precomputing these quantities like is done in exact quantum dynamics. 

To avoid this we can approximate the integral of a property by taking the taylor series expansion. And because these are gaussian integrals we can take advantage of the Gaussian product theorem which tells us that the first order term is the centroid between the two TBFS.

## Backpropagation
Backpropagate to $t_{entry}$ to better describe transfer of amplitude

Backpropagation is a method used in AIMS to better account for the non-adiabatic transition event, i.e., the "spawning" event, where a child trajectory is born from a parent trajectory due to non-adiabatic coupling. 

In principle, spawning could happen at any point between two time steps when the coupling is above a certain threshold. However, in practice, the simulation can only check for spawning events at each time step. This could lead to inaccuracies if the maximum coupling (and hence the most likely spawning point) is missed. 

To address this, AIMS introduces the backpropagation scheme, which works as follows:

1. Once a spawning event is detected at a certain time step, the simulation first backpropagates both the parent and the child trajectories to the time of entry into the spawning zone (t_entry), which is defined as the region of configuration space where the non-adiabatic coupling exceeds a certain threshold.

2. The simulation then searches for the time of maximum coupling (t_max) between t_entry and the current time. 

3. The child trajectory is then "reborn" at t_max with the appropriate phase and amplitude. The parent trajectory is also adjusted to reflect the loss of amplitude due to the spawning event.

This backpropagation scheme aims to more accurately describe the transfer of amplitude from the parent to the child trajectory, leading to improved accuracy in the description of non-adiabatic dynamics. It takes into account that the spawning event is a continuous process and not just a single event happening exactly at the time steps of the simulation. This method helps to alleviate the "quantization" of the spawning process inherent in the numerical treatment and results in more accurate dynamics.


## Norm Preserving Integration
Norm-preserving integration is an important aspect in methods like Ab Initio Multiple Spawning (AIMS) that deal with non-adiabatic dynamics and spawn new Trajectory Basis Functions (TBFs). 

Norm in this context refers to the total probability, or the integral of the absolute square of the wavefunction, which should be conserved throughout the dynamics. In a quantum mechanical system, the norm of the wavefunction corresponds to the total probability of finding the system in any state, and as such, must always be equal to 1. 

However, when trajectories are spawned in AIMS, it's possible for the norm to increase, as each new TBF could potentially contribute additional probability. To maintain the correct total norm, a procedure known as norm-conserving or norm-preserving integration is used.

In the norm-preserving integration, spawning events are handled in a way that preserves the total norm. This can be done by adjusting the amplitudes of the parent and child trajectories during spawning. When a new TBF is spawned, some probability amplitude is transferred from the parent TBF to the child TBF. The amplitude of the parent trajectory is decreased to account for the amplitude given to the child trajectory. 

In principle, if the spawning is done correctly and all trajectories are propagated correctly, the total norm will be conserved. In practice, however, due to numerical errors and approximations, norm conservation might not be exact, and additional norm-conservation or norm-preserving steps might be necessary.

Norm-preserving integration is a critical step in ensuring that the AIMS method, and similar quantum dynamics methods, correctly represent the quantum mechanical system and provide physically meaningful results. Without it, the total probability could artificially increase or decrease, leading to unphysical results.

## Important parameters
`overlap_thresh` controls the calculation of centroids via the saddle point approximation between TBFs
—> Greatly reduces number of calculations between TBFs

`popspawn`

`csthresh`

try with cfthres=csthresh