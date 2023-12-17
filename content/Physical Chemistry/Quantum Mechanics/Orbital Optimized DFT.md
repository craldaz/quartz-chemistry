---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Orbital Optimized DFT]]
--- 

- What led me here: [[Density Functional Theory]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

[[Diptharka Hait]]

Modeling Excited States

Optimizing excited-state orbitals

Variational Collapse makes it difficult to get excited-state specific orbitals
Optimization often instead leads to a nearby minimum like the ground state

Square gradient minimization

Find some set of orbitals $\theta$ corresponding to a desired non-Aufbau (excited state) electronic configuration such that the energy E(theta) is stationary vs theta without collapsing to another state

All stationary points are global minima of $\Delta=|\nabla_{\theta} E|^2$
Need the gradient of $\Delta$, not much more expensive than doing 

Does really good for x-ray (Orbital Optimized ROKS can get < 0.5 RMS error) excitation energy

## Feedback
Ground-State quantum chemistry slide (too many bullet points)

Kind of strange to note the applications several slides in. Would it be better to introduce this at the beginning?


