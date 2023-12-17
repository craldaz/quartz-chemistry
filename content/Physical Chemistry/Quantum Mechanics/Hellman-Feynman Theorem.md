---
tags: 🧪
---
# `Title:` [[Hellman-Feynman Theorem]]
--- 

The **Hellmann–Feynman theorem** relates the derivative of the total energy with respect to a parameter, to the [expectation value](https://en.wikipedia.org/wiki/Expectation_value_(quantum_mechanics)) of the derivative of the [Hamiltonian](https://en.wikipedia.org/wiki/Hamiltonian_(quantum_mechanics) "Hamiltonian (quantum mechanics)") [[Hamiltonian]] with respect to that same parameter.


This is very important for calculating intramolecular forces (i.e. nuclear energy gradients).


A simple example can be calculated using Tully's Simple avoided crossing model: 

```python
 ## \f$V(x)\f$
    def V(self, x):
        v11 = m.copysign(self.A, x) * ( 1.0 - m.exp(-self.B * abs(x)) )
        v22 = -v11
        v12 = self.C * m.exp(-self.D * x * x)
        out = np.array([ [v11, v12],
                         [v12, v22] ])
        return out

    ## \f$\nabla V(x)\f$
    def dV(self, x):
        v11 = self.A * self.B * m.exp(-self.B * abs(x))
        v22 = -v11
        v12 = -2.0 * self.C * self.D * x * m.exp(-self.D * x * x)
        out = np.array([ [v11, v12],
                         [v12, v22] ])
        return out.reshape([2, 2, 1])
```

https://en.wikipedia.org/wiki/Hellmann–Feynman_theorem




[[Quantum Mechanics]]
