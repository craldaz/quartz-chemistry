---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Trotterization]]
--- 

- What led me here: [[Quantum Dynamics]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```


## Spectral Decomposition
$$U(t) = \sum_n exp(-iE_nt)\ket{n}\bra{n}$$
$$A-> \lambda_nV_n$$
- Diagonalization cubic cost for number of basis states ON^3
- What N is needed for the lowest M edge states? 
- If our basis were true eigenstates N=M (eigenstates that we think we need to represent Hamiltonian)

## Trotterization
Splitting the propagator
$U(t) = exp(-iHt) = exp(-iTt)exp(-iVt) + O(t^2)$
Only good to second order in time step s. Erro

We can break the propagate up into little bits by defining $\Delta t = t/N$ 

Local error is 
$$[T,V](t/N)^2$$ Global error from N steps $O(\Delta t)$
Trot our way to solution 
Trotter equation https://mathworld.wolfram.com/TrotterProductFormula.html

If $\Delta t$ is very small it might compete with round-off error in a computer. So be careful. 

Need ~5-10 points for fastest period of frequency of system
1 femtosecond time-steps 
2 femtosecond time step is too large? 

Time step is usually shorter for quantum system 
Trotterization, named after a person Hale Trotter

However, this is not time reversible, VT is not the same as TV. Time going forward is different than going backward. Time reversibility is the same as energy conservation. 

$U^T(\Delta t) = U(-\Delta t)$

(AB)^T = B^T A^T

## Trotter-Suzuki Formula
Symmetric Formula
$$e(-iV\Delta t/2)e(-iT\Delta t)e(-iV\Delta t/2)$$

## Split Operator Fourier Transform
Relies on [[Fourier Transform]] scales as NLogN
Much faster than diagonalizing full Hamiltonian N^3
Special case of the pseudo-spectral method. One-basis is great for one part of one  equation, one-basis is great for another part of one equation. Use both! Better to pay transformation cost, than to live with non-ideal diagonalization. 

Everyone in electromagnetic radiation studies would use this method, EM has the advantage that it is only three dimensional. 100 dimensional FT is not as easy. 



