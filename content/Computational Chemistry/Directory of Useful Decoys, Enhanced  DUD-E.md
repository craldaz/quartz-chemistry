---
cssClass:
- wide
tags:
  - 🧪
---

# `Title:` [[Directory of Useful Decoys, Enhanced  DUD-E]]
--- 

- What led me here: [[Drug Discovery]] [[Machine Learning]]

Inlinks
```dataview 
list from [[#this.file.name]] and !outgoing([[# this.file.name]]) 
```

# Directory of Useful Decoys, Enhanced (DUD-E)

## Overview

The Directory of Useful Decoys, Enhanced (DUD-E) is a database designed to assist researchers in the field of computational drug discovery. It contains a collection of molecular decoys for a broad range of protein targets. A decoy, in this context, is a molecule that is structurally similar to an active ligand but does not bind to the protein target. DUD-E aims to facilitate the development and validation of docking algorithms, scoring functions, and virtual screening methods by providing a benchmark set of decoys.

## Features

- Contains over 22,000 active compounds for 102 targets.
- Each active compound is paired with 50 property-matched decoys.
- Designed to evaluate the performance of docking algorithms.
- Includes targets from diverse protein families, such as kinases, phosphatases, and proteases.

## Applications in Predicting Activity of Drugs

### As a Benchmark Tool
The DUD-E database can serve as a benchmark for new machine learning models designed to predict the activity of drugs. By comparing the model's performance on both active compounds and decoys, researchers can more accurately assess the predictive power of their algorithms.

### Handling Imbalanced Datasets
For researchers like Cody Aldaz, who specialize in machine learning and have expertise in chemistry, one common problem is the lack of a large set of negative or decoy examples for training models. DUD-E can help to mitigate this issue by providing a large, publicly available set of decoys.

### Advanced Algorithms
With a strong foundation in algorithms and graph theory, you could explore complex features and representations of these decoys, potentially uncovering novel patterns or characteristics that simpler models may overlook.

## Are Decoys Simply Negatives?

While it might be tempting to label all decoys as negatives, caution is advised. The definition of a decoy in DUD-E is specific; these molecules are carefully selected to be similar in properties to active ligands but are non-binding. Simply labeling them as negatives could introduce false positives in your model evaluation if not properly accounted for. Given your deep understanding of chemistry, you might consider additional analyses to validate that these decoys are true negatives for your specific research question.

## Conclusion

DUD-E is a valuable resource for researchers in the field of computational drug discovery, particularly for those interested in developing or validating algorithms for predicting drug activity. It provides a rich set of decoys that can be used to balance datasets and improve the reliability of predictive models. However, due care should be exercised when using these decoys as negative examples, to avoid potential issues with false positives.

---

For those with a strong background in both computer science and chemistry, such as Cody Aldaz, DUD-E offers a valuable set of data for developing more robust and reliable machine learning models aimed at predicting drug activity.