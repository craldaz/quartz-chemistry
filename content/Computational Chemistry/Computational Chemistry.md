---
tags: 🧪
---
# `Title:` [[Computational Chemistry]]
--- 

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

[[index]]
# Computational Chemistry

Computational chemistry is a branch of chemistry that uses computer simulation to assist in solving chemical problems. It uses methods of theoretical chemistry, incorporated into efficient computer programs, to calculate the structures and properties of molecules and solids.

## Overview

Computational chemistry can involve the computation of molecular structures, the calculation of electronic properties, the simulation of chemical reactions, and the prediction of the behavior of molecules. It can be used to predict the properties of molecules that have not yet been synthesized, to explore the mechanisms of chemical reactions, and to design new drugs and materials.

The methods used in computational chemistry include molecular mechanics, quantum mechanics (QM), and molecular dynamics (MD). These methods can be used separately or in combination, depending on the problem to be solved.

## Applications

Computational chemistry has a wide range of applications. It is used in the design of new drugs and materials, in the study of environmental chemistry, in the understanding of the fundamental nature of chemical reactions, and in many other areas of research in chemistry and biochemistry.

## See Also

- Quantum Chemistry
- Molecular Mechanics
- Molecular Dynamics

## References

1. Leach, Andrew R. (2001). Molecular Modelling: Principles and Applications (2nd ed.). Prentice Hall.
2. Jensen, Frank (2007). Introduction to Computational Chemistry (2nd ed.). John Wiley & Sons.

---

This article incorporates text available under the CC BY-SA 3.0 license.

```dataviewjs
let page = dv.current().file.path;
let pages = new Set();
let stack = [page]; 
while (stack.length > 0) {
	let elem = stack.pop();
	let meta = dv.page(elem);
	if (!meta) continue; 
		for (let inlink of meta.file.inlinks.concat(meta.file.outlinks).array()) { console.log(inlink);
		if (pages.has(inlink.path)) continue;
		pages.add(inlink.path);
		stack.push(inlink.path); 
	}
} // Data is now the file metadata for every page that directly OR indirectly links to the current page. 
let data = dv.array(Array.from(pages)).map(p => dv.page(p));
```
