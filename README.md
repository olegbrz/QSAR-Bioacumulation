# QSAR-Bioacumulation

This project is an implementation written in R of a scheme to predict whether a compound is

- Mainly stored within lipid tissues
- Has additional storage sites (e.g., proteins)
- Is metabolized/eliminated with a reduced bioconcentration

The approach is based on two validated QSAR (Quantitative Structure–Activity Relationship) trees, whose salient features are descriptor interpretability and simplicity.

The scheme is based on the following paper: [Investigating the mechanisms of bioconcentration through QSAR classification trees](https://pubmed.ncbi.nlm.nih.gov/26760717/)

## Dataset

The dataset has the following fields:

3 Compound identifiers:

- CAS number
- Molecular SMILES
- Train/test splitting

9 molecular descriptors (independent variables):

- nHM
- piPC09
- PCD
- X2Av
- MLOGP
- ON1V
- N-072
- B02[C-N]
- F04[C-O]

2 experimental responses:

- Bioconcentration Factor (BCF) in log units (regression)
- Bioaccumulation class (three classes)