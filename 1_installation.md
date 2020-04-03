---
layout: page
title: Installation
---

You can either install the BioConductor version or the development version from GitHub.
```r
# install from bioconductor
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install("dorothea")

# install the development version from GitHub
# install.packages("devtools")
devtools::install_github("saezlab/dorothea")


```

