# WeberDivechaLCdata

[![R build status](https://github.com/lmweber/WeberDivechaLCdata/workflows/R-CMD-check-bioc/badge.svg)](https://github.com/lmweber/WeberDivechaLCdata/actions)


This package contains data from our paper on the single-nucleus and spatially-resolved landscape of gene expression in the human locus coeruleus (LC).

The package is available from Bioconductor ([WeberDivechaLCdata](https://bioconductor.org/packages/WeberDivechaLCdata)).

Datasets are stored in R/Bioconductor formats ([SingleCellExperiment](https://bioconductor.org/packages/SingleCellExperiment) and [SpatialExperiment](https://bioconductor.org/packages/SpatialExperiment)).

The paper is available from [eLife](https://elifesciences.org/articles/84628).


## Installation

The data package is available from Bioconductor ([WeberDivechaLCdata](https://bioconductor.org/packages/WeberDivechaLCdata)) and can be installed as follows:

```
install.packages("BiocManager")
BiocManager::install("WeberDivechaLCdata")
```


## Contents

The package contains two objects:

- 1x [SpatialExperiment](https://bioconductor.org/packages/SpatialExperiment) formatted R object containing the SRT data
- 1x [SingleCellExperiment](https://bioconductor.org/packages/SingleCellExperiment) formatted R object containing the snRNA-seq data


## Loading the data

The R/Bioconductor data objects can be loaded as follows:

```
library(SpatialExperiment)
library(SingleCellExperiment)
library(WeberDivechaLCdata)

# Load objects using dataset names
spe <- WeberDivechaLCdata_Visium()
sce <- WeberDivechaLCdata_singleNucleus()

# Show objects
spe
sce
```

More details including alternative ways to load the data and details on the data structure are provided in the package vignette, which can be found on the Bioconductor package page ([WeberDivechaLCdata](https://bioconductor.org/packages/WeberDivechaLCdata)) or directly [here](https://bioconductor.org/packages/release/data/experiment/vignettes/WeberDivechaLCdata/inst/doc/WeberDivechaLCdata.html).


## Citation

- Weber L.M.\*, Divecha H.R.\*, Tran M.N., Kwon S.H., Spangler A., Montgomery K.D., Tippani M., Bharadwaj R., Kleinman J.E., Page S.C., Hyde T.M., Collado-Torres L., Maynard K.R., Martinowich K.\*, and Hicks S.C.\* (2023). *The gene expression landscape of the human locus coeruleus revealed by single-nucleus and spatially-resolved transcriptomics.* [eLife](https://elifesciences.org/articles/84628), 12:RP84628.
