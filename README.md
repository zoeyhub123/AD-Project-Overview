# AD-Project-Overview

This repository contains the R code and documentation for subtyping alzheimer diseases (AD) using NACC data.

## **Overview**

### Filtering:

* AD group (Braak stage for neurofibrillary degeneration (NACCBRAA) == 3 or 4, and Density of neocortical neuritic plaques (NACCNEUR)== 2 or 3, and Lewy body pathology (NACCLEWY) == 0 or 1), and
* Mixed AD group (Braak stage for neurofibrillary degeneration (NACCBRAA) == 3 or 4, and Density of neocortical neuritic plaques (NACCNEUR)== 2 or and Lewy body pathology (NACCLEWY) == 3)
* Others: label == 99


### Visualizations:

* Histograms and barcharts are generated to show the distribution and missing value of each variables.

### Data Joining & Reshaping:

* Five datasets (UDS, MRI, CSF, MRIQC, MRISBM) are merged into a joined subset.
* To manage sparsity, visits within different window are grouped (such as 6months, 1year, 2year, and 1000 days), and overlapping dates are aggregated by keeping the first observation (this can be modified).

### Requirements

* R with the packages: dplyr, data.table, ggplot2, knitr, purrr, tidyr, stringr, tibble, lubridate

### Reference:

* Codebooks can be seen under the main directory.

* https://alz-journals.onlinelibrary.wiley.com/journal/15525279
* For further detail, please contact ziyi48945@gmail.com
