---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[OpenMolcas]]
--- 

- What led me here: [[Computational Chemistry Software]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

Not too familiar with this package but they have a docker container. 

```

&Gateway 
    Coord  
    3  
    Angstrom
    O  0.00  0.00  0.00
    H  0.75  0.00  0.50
    H  0.75  0.00  -0.50
    Group = NoSym 
    Basis = 6-31G*

&Seward

&Scf
```


```
docker   run    -v   $PWD:/home/     steabert/openmolcas     /home/molcas.input
```

[[Docker]]