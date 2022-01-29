### ENIGMA analysis
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5906932.svg)](https://doi.org/10.5281/zenodo.5906932)

To reproduce main parts of the simulations and analysis results in our manuscript, here we give several example code for data simulation and analysis.
tips:
1. Before users run following example, user need to source the ENIGMA code at first
```
source("ENIGMA.R")
```
2. Before running the CTS-DE analysis, user need to source related functions
```
source("DEG_analysis_uile_function.R")
```
Both scripts could be downloaded through following links:

[ENIGMA.R](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/ENIGMA.R)

[DEG_analysis_uile_function.R](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/DEG_analysis_uile_function.R)

## Code for main text
### Simulation analysis
* [Using tumor scRNA-seq data to simulate pseudo-bulk sample and perform deconvolution](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/Simulation%20(scRNA-seq).R)

* [Simulate cell type-specific gene expression profile to assess CTS-DEGs detection accuracy](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/Simulation%20(DEG).R)

  [Benchmark CTS-DEG detection performance](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/DEG_analysis.R)

* [Identify four latent cell senescence states in Fibroblast](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/latentCellState.R)

* [Identify cell type specific pseudo-trajectory](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/ESCO_path.R)

### Real Data analysis
#### Deconvolution analysis for arthritis patients(HTML format): 
* [link](https://htmlpreview.github.io/?https://github.com/WWXkenmo/ENIGMA/blob/main/ENIGMA_analysis/Real_Data_Analysis/RA/Deconvolution-Analysis-for-Arthritis-Patients.html)
#### Deconvolution analysis for T2D patients(HTML format): 
* [Part-1](https://htmlpreview.github.io/?https://github.com/WWXkenmo/ENIGMA/blob/main/ENIGMA_analysis/Real_Data_Analysis/pancreas/The-deconvolution-analysis-in-pancreas-islet-tissues.html)
* [Part-2](https://htmlpreview.github.io/?https://github.com/WWXkenmo/ENIGMA/blob/main/ENIGMA_analysis/Real_Data_Analysis/pancreas/Beta-cell-type-specific-network-in-pancreas-islet-tissues.html)

## Code for supplementary note
#### 1. [Using COVID-19 PBMC single cell datasets to explain the role of parameter alpha](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/Simulation(mutilPaltforms).R) (Supplementary Figure N8)

#### 2. [Attaching noise to reference profile to explain the role of parameter alpha through CTS-DE analysis](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/ADMM_noise.R) (Supplementary Figure N7)

#### 3. [Remove the spurious correlations betweeen inferred CSE profiles and cell type fractions](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/Normalize_celltype_fractions.R) (Supplementary Figure N9,N10,N11)

#### 4. [Post-hoc nonnegative constraint](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/NegativeValueEffects.R) (Supplementary Figure N2, N13, N14)

#### 5. [Using gradient renormalized maximum L2 norm model improve the performance](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/Renomarlization_solver_compare_new.R) (Supplementary Figure N3,N4,N15)
  Note: we also write a [document](https://github.com/WWXkenmo/ENIGMA/blob/master/vignettes/Why-fixed-renormalized-gradient-norm-size-%3D-200.pdf) to introduce why we use 200 as the new gradient norm size of renormalized gradient.
  
#### 6. [The role of theta_hat factor in trace norm model](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/ENIGMA_Script/loss_design_explain.R) (Supplementary Figure N5)

#####  DataSets: 
1. [Datasets for DEG analysis](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/Data/DEG_example_data)
2. [Datasets for cell state identification](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/Data/CellStateIdentification)
3. [Datasets for sample/gene-level correlation analysis](https://github.com/WWXkenmo/ENIGMA_analysis/tree/main/ENIGMA_analysis/Data/CSE_correlation)
