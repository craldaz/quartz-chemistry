---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Stochastic Selection AIMS]]
--- 

- What led me here: [[Ab Initio Multiple Spawning]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

Stochastic Selection Ab Initio Multiple Spawning (SS-AIMS) is a computational approach used in quantum dynamics simulations of chemical reactions. It is based on the idea of using a stochastic algorithm to select the most relevant electronic states during the simulation, and spawning new trajectories from those states.

The SS-AIMS methodology is used to simulate nonadiabatic processes, which involve transitions between electronic states of a molecule during a chemical reaction. In traditional methods, all electronic states are propagated simultaneously, which can be computationally expensive and unnecessary since some states may not be relevant to the reaction of interest. SS-AIMS, on the other hand, selects a subset of the most important states to propagate, significantly reducing computational costs.

The selection of states in SS-AIMS is done using a statistical approach, where the probability of selecting a particular electronic state is proportional to its contribution to the overall wave function. By selecting the most relevant states at each time step, SS-AIMS can accurately simulate complex molecular processes, including those involving multiple electronic states and nonadiabatic transitions.

Here is how it works:
> The three TBFs on the left are coupled, while the one on the right is only weakly coupled to the third TBF. (b) The stochastic-selection algorithm detects the weak coupling (coupling is below the threshold ε) and forms two uncoupled blocks of coupled trajectories (3 TBFs in the first block, 1 in the other). (c) A random number is generated and one of the blocks is selected (with selection probability proportional to the population in the block). In this example, the first block is selected. The unselected blocks (the fourth TBF in this example) are then removed from the simulation and the population of each TBF in the selected block is scaled to maintain normalization of the wave function. The nonadiabatic dynamics then proceeds with only TBFs from the selected block.


>  In many multidimensional problems, TBFs will not come close to each other after separating. In that case, the union of all the TBFs created in the mother/daughter/granddaughter simulations will replicate the results that would have been obtained without simulation splitting.

SS-AIMS has been shown to be an effective and efficient approach for simulating a wide range of chemical reactions, including photochemical processes, radiation damage in biological molecules, and more.

Need to repeat the SS-AIMS multiple times since its stochastic  

ESSAIMS: Energy 
OSSAIMS: Overlap

ESSAIMS:
> Let us nowdefine more precisely what we mean by uncoupled. In the following, we will compare the absolute value of the matrix elements H_kl (both H_kl^{IJ} and H_kl^{II}) with a threshold criterion to determine whether trajectories can be considered uncoupled. Hence, the stochastic selection will be applied on truly uncoupled TBFs only if a sufficiently small threshold is selected. On the other hand, we can relax the definition of uncoupled TBFs and perform the stochastic selection more often by employing a larger threshold. The resulting reduced number of TBFs in the dynamics comes at the cost of neglecting the effect of nonvanishing interference terms. Since the proposed criterion has an energy unit, we label the resulting stochastic-selection AIMS method as ESSAIMS.

ESSAIMS reduces by a factor of 3 the average number of electronic structure calls per run with respect to AIMS: 1068 for AIMS (average over 39 initial conditions) compared to 316 for ESSAIMS (average over 194 runs, ε = 10−3 a.u.

In a different paper they observed that OSAIMS might be a bit better because the Independent First Generation, the overlap is less system dependent. (Just a number between 0 and 1, might have to scale for size but probably possible)

If the dynamics have super weak coupling than it is even worse than surface hopping. 

There is a new solution that Basile and Yorick are working on


1. "SSAIMS-Stochastic-Selection Ab Initio Multiple Spawning for Efficient Nonadiabatic Molecular Dynamics" published in the Journal of Physical Chemistry A in 2020.
2.  "Comparing (Stochastic-Selection) Ab Initio Multiple Spawning with Other Nonadiabatic Dynamics Models" published in Chemical Reviews in 2021.
3. "AIMS-WISS: Ab Initio Multiple Spawning with Informed Stochastic Search" published in the Journal of Chemical Theory and Computation in 2021.
4. "Theoretical Number of Electronic Structure Calculations at Each Time Step in Nonadiabatic Dynamics Simulations: Multiplication, Ab Initio and Stochastic" published in Chemical Science in 2021.