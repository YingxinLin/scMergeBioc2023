
# Atlas-scale single-cell multi-sample multi-condition data integration using scMerge2


## Overview


The recent emergence of multi-sample multi-condition single-cell multi-cohort studies allows researchers to investigate different cell states. The effective integration of multiple large-cohort studies promises biological insights into cells under different conditions that individual studies cannot provide. 

### Description

With the rapid emergence of multi-sample multi-condition single-cell studies and the increased number of datasets for integration, our proposed scMerge2 addresses challenges associated with scalability of cells and studies as well as producing analytically ready data (i.e. adjusted expression matrix). This is achieved via three key innovations compared to the previous version of scMerge:

1. Hierarchical integration is used to capture both local and global variation. scMerge2 provides users with a more flexible and adaptable multi-level merging structure, of which each level can comprise multiple collections of several batches and batch correction can be performed within each collection separately using user-defined batch labels. 

2. Pseudo-bulk construction is used to reduce computing load, allowing for the analysis of datasets containing millions of cells. 

3. Pseudo-replication inside each condition is built, allowing for the modelling of numerous conditions. 

In essence, scMerge2 takes gene expression matrices from a collection of datasets and integrates them in a hierarchical manner. The final output of scMerge2 is a single adjusted expression matrix with all input data matrices merged and ready for downstream analysis.


### Pre-requisites

It is expected that students will have:

1. Basic knowledge of R syntax
2. Familiarity with `SingleCellExperiment` objects


### Participation

While it will be possible for participants to run code as we go through the demonstration, given time constraints, I would encourage them to focus their attention into integration strategies behind scMerge2 (pseudo-replicates, pseudo-bulk, stably expressed genes, number of unwatned variation factors and hierarchical mering etc.). Questions are welcome both within the workshop and if participants choose to work through the workshop independently after the demonstration.


### _R_ / _Bioconductor_ packages used

This workshop will focus on Bioconductor packages scMerge and [SingleCellExperiment] (https://bioconductor.org/packages/release/bioc/html/SingleCellExperiment.html).


### Time outline

An example for a 45-minute workshop:

| Activity                     | Time |
|------------------------------|------|
| Introduction of method       | 10m  |
| Introduction of core function| 10m  |
| Hierarchical merging         | 10m  |
| Best practise                | 10m  |


### Workshop

The detailed workshop materials can be found in this link: https://yingxinlin.github.io/scMergeBioc2023.


### Reference


1. scMerge: **scMerge leverages factor analysis, stable expression, and
pseudoreplication to merge multiple single-cell RNA-seq datasets**. Yingxin Lin, Shila Ghazanfar, Kevin Y.X. Wang, Johann A. Gagnon-Bartsch,
Kitty K. Lo, Xianbin Su, Ze-Guang Han, John T. Ormerod, Terence P.
Speed, Pengyi Yang, Jean Y. H. Yang. (2019). Our manuscript published at PNAS can be found
[here](http://www.pnas.org/lookup/doi/10.1073/pnas.1820006116).

2. scMerge2: **Atlas-scale single-cell multi-sample multi-condition data integration using scMerge2**. Yingxin Lin, Yue Cao, Elijah Willie, Ellis Patrick, Jean Y.H. Yang. (2023). Our manuscript published in Nature Communications can be found [here](https://doi.org/10.1038/s41467-023-39923-2).


