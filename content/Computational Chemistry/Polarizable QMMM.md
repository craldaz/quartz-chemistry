---
tags: 🧪
---
# `Title:` [[Polarizable QMMM]]
--- 
[[Ab Initio Methods]]
[[Henry Wang]] gave a talk on the work that he is doing with [[Michael Miller]] and [[Alessio Valentini]] on polarizable QM/MM in Tinker and TeraChem.

The specific model is known as the induced dipole model. Apparently this technique is superior to the drude oscillator model.

It looks like an SCF problem because the induced dipoles induce dipoles in the other induced dipoles. So it must be solved self-consistently. 

The polarization energy is related to the difference between a system w/ a polarizable atom and an induced dipole, and no induced dipole. 

The induced dipole is converged when the derivative of the polarization energy is zero with respect to the dipole.

--> Find the induced dipole which minimizes the polarization energy. 

I posted a question on Stack Exchange asking about the polarization catastraphe.
https://mattermodeling.stackexchange.com/q/6458/52

