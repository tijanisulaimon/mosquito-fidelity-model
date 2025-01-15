# The potential impacts of vector host species fidelity on zoonotic arbovirus transmission


**Tijani A. Sulaimon** ([ORCID](https://orcid.org/0000-0002-9735-8548))<sup>1,2,4,*</sup>, **Anthony J. Wood** ([ORCID](https://orcid.org/0000-0001-9973-8205))<sup>2</sup>, **Michael B. Bonsall** ([ORCID](https://orcid.org/0000-0003-0250-0423))<sup>3</sup>, **Michael Boots** ([ORCID](https://orcid.org/0000-0003-3763-6136))<sup>5</sup>, **Jennifer S. Lord** ([ORCID](https://orcid.org/0000-0001-6616-1526))<sup>6, *</sup>  

<sup>1</sup> Royal (Dick) School of Veterinary Studies, University of Edinburgh, Easter Bush Campus, Midlothian, EH25 9RG, United Kingdom  
<sup>2</sup> The Roslin Institute, University of Edinburgh, Easter Bush Campus, Midlothian, EH25 9RG, United Kingdom  
<sup>3</sup> Department of Biology, University of Oxford, Oxford, United Kingdom  
<sup>4</sup> African Institute for Mathematical Sciences (AIMS), Cape Town, South Africa  
<sup>5</sup> Department of Integrative Biology, University of California, Berkeley, California, USA  
<sup>6</sup> Department of Vector Biology, Liverpool School of Tropical Medicine, Liverpool, United Kingdom  

**Correspondence**: [tijani@aims.ac.za](mailto:tijani@aims.ac.za)


## Abstract
The interaction between vector host preference and host availability on vector blood feeding behaviour has important implications for the transmission of vector-borne pathogens. However, to our knowledge, the effect of bias towards feeding on the same host species from which a first meal was taken, termed fidelity, has not been quantified. Using a mathematical model we showed that vector fidelity to the host species they take a first blood meal from leads to non-homogeneous mixing between hosts and vectors. Taking Japanese encephalitis virus (JEV) as a case study, we investigated how vector preference for amplifying vs dead-end hosts and fidelity can influence JEV transmission. We show that in regions where pigs (amplifying hosts) are scarce compared to cattle (dead-end hosts preferred by common JEV vectors), JEV can still be maintained through vector fidelity. Our findings demonstrate the importance of considering fidelity as a potential driver of transmission, particularly in scenarios such as Bangladesh and India where the composition of the host community might initially suggest that transmission is not possible.

This papaer has been published in ...

## Contents
- `scripts/`: contains all code for analyzing the model. Brief descriptions of each file:

  - **model.R**: Core model functions, \(R_0\) function, and likelihood function for parameter estimation

  - **parameters.R**: Defines all model parameters

  - **r0LHSsensitivity_JSL.R**: performs global sensitivity analysis of \(R_0\) using Latin Hypercube Sampling (LHS)

  - **simulate.R**: Runs simulations, explores \(R_0\) values, and includes mosquito feeding experiments
- `figures/` - Plots and tables generated for the paper

## Getting Started
To run the model:  
1. Open `simulate.R`.  
2. Source the model functions from `model.R`
3. Ensure all required libraries are installed

```R
sessionInfo()
R version 4.4.2 (2024-10-31)
Platform: x86_64-apple-darwin20
Running under: macOS Sequoia 15.2

Matrix products: default
BLAS:   /System/Library/Frameworks/Accelerate.framework/Versions/A/Frameworks/vecLib.framework/Versions/A/libBLAS.dylib 
LAPACK: /Library/Frameworks/R.framework/Versions/4.4-x86_64/Resources/lib/libRlapack.dylib;  LAPACK version 3.12.0

locale:
[1] en_US.UTF-8/en_US.UTF-8/en_US.UTF-8/C/en_US.UTF-8/en_US.UTF-8

attached base packages:
[1] parallel  grid      stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] deSolve_1.40     leaflet_2.2.2    kableExtra_1.4.0 lubridate_1.9.3  forcats_1.0.0   
 [6] stringr_1.5.1    dplyr_1.1.4      purrr_1.0.2      readr_2.1.5      tidyr_1.3.1     
[11] tibble_3.2.1     ggplot2_3.5.1    tidyverse_2.0.0  here_1.0.1       lhs_1.2.0       
[16] gridExtra_2.3    reshape_0.8.9   

loaded via a namespace (and not attached):
 [1] utf8_1.2.4         generics_0.1.3     xml2_1.3.6         stringi_1.8.4      hms_1.1.3         
 [6] digest_0.6.37      magrittr_2.0.3     RColorBrewer_1.1-3 evaluate_1.0.1     timechange_0.3.0  
[11] fastmap_1.2.0      rprojroot_2.0.4    plyr_1.8.9         backports_1.5.0    crosstalk_1.2.1   
[16] viridisLite_0.4.2  scales_1.3.0       cli_3.6.3          rlang_1.1.4        munsell_0.5.1     
[21] withr_3.0.2        tools_4.4.2        reshape2_1.4.4     tzdb_0.4.0         colorspace_2.1-1  
[26] broom_1.0.7        vctrs_0.6.5        R6_2.5.1           lifecycle_1.0.4    htmlwidgets_1.6.4 
[31] pkgconfig_2.0.3    pillar_1.10.0      gtable_0.3.6       glue_1.8.0         Rcpp_1.0.13-1     
[36] systemfonts_1.1.0  xfun_0.49          tidyselect_1.2.1   rstudioapi_0.17.1  knitr_1.49        
[41] xtable_1.8-4       farver_2.1.2       htmltools_0.5.8.1  labeling_0.4.3     rmarkdown_2.29    
[46] svglite_2.1.3      compiler_4.4.2    
