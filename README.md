# AHBA Epilepsy
Transcriptomic analysis of regions showing cortical thinning in the common epilepies.

This repository contains code for the paper entitled:
*A systems-level analysis highlights microglial activation as a modifying factor in common epilepsies*. 
The pre-print is available here: https://www.biorxiv.org/content/10.1101/470518v1

To run this repository following external files are required:
* Allen Institute for Brain Sciences (AIBS) human brain atlas (AHBA) microarray gene expression data: http://human.brain-map.org/static/download
* AHBA RNA-seq data: http://human.brain-map.org/static/download
* Updated MNI cooridnates: https://github.com/chrisgorgo/alleninf/tree/master/alleninf/data

Cell-type fractions were obtained from SSMI scaled data using Scaden (10.1126/sciadv.aba2619), the fractions are contained within the data folder in this repository.

One jupyter notebook deals with the selection and re-scaling of geneexpression data to produce SSMI (sequencing scaled microarray intensities) as described by Miller et al. (2014) http://www.biomedcentral.com/1471-2164/15/154

The second notebook performs the association analyses for (1) cell type fractions and for (2) log2(SSMI) per gene using a linear mixed effects models.
