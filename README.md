> [!WARNING]
> This repository has been archived and is no longer maintained.  
> The code is provided for historical reference and may contain unpatched or unknown vulnerabilities.  
> It should not be used in production systems.  

[![Build Status](https://travis-ci.com/ashishjain1988/MAFDash.svg?branch=master)](https://app.travis-ci.com/github/ashishjain1988/MAFDash)
![GitHub release (latest by date)](https://img.shields.io/github/v/release/ashishjain1988/MAFDash)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6195233.svg)](https://doi.org/10.5281/zenodo.6195233)
<!--
[![CRAN status](https://www.r-pkg.org/badges/version/MAFDash)](https://cran.r-project.org/package=MAFDash)
![Downloads](https://cranlogs.r-pkg.org/badges/MAFDash)
![Total Downloads](https://cranlogs.r-pkg.org/badges/grand-total/MAFDash)
[![Codecov test coverage](https://codecov.io/gh/ashishjain1988/MAFDash/branch/main/graph/badge.svg)](https://app.codecov.io/gh/ashishjain1988/MAFDash?branch=main)
![GitHub all releases](https://img.shields.io/github/downloads/ashishjain1988/MAFDash/total)
[![R-CMD-check](https://github.com/ashishjain1988/MAFDash/workflows/R-CMD-check/badge.svg)](https://github.com/ashishjain1988/MAFDash/actions)-->

MAFDash
------------------------------------------------------------
*Once you call the variants, it's a MAFDash to the finish line*


**An easy-to-use dashboard builder for mutation data**

*[View documentation on github.io](https://ashishjain1988.github.io/MAFDash/index.html)*

### Installation from Github
```
# install.packages(devtools)  ## Install devtools if necessary
devtools::install_github("ashishjain1988/MAFDash")
```

<!--### Installation from CRAN
```
install.packages("MAFDash")
```
-->

### Description
[Mutation Annotation Format (MAF)](https://docs.gdc.cancer.gov/Encyclopedia/pages/Mutation_Annotation_Format/) is a tabular data format used for storing genetic mutation data. For example, [The Cancer Genome Atlas (TCGA)](https://www.cancer.gov/about-nci/organization/ccg/research/structural-genomics/tcga) project has made MAF files from each project publicly available.

MAFDash is an R package that helps to quickly create an HTML dashboard to summarize and visualize data from MAF files. The resulting HTML file serves as a self-contained report that can be used to explore and share the results.

Currently, MAFDash produces mostly static plots powered by [maftools](https://bioconductor.org/packages/release/bioc/vignettes/maftools/inst/doc/maftools.html),  [ComplexHeatmap](https://github.com/jokergoo/ComplexHeatmap) and [circlize](https://github.com/jokergoo/circlize), as well as interactive visualizations using [canvasXpress](https://cran.r-project.org/package=canvasXpress) and [plotly](https://plotly.com/r/).  The report is generated with a parameterized [R Markdown](https://rmarkdown.rstudio.com/) script that uses [flexdashboard](https://pkgs.rstudio.com/flexdashboard/) to arrange all the information.

### How to use

- [Quick Start](https://ashishjain1988.github.io/MAFDash/articles/Quick_Start.html)
- [Customizing](https://ashishjain1988.github.io/MAFDash/articles/Customizing.html)
- [Real-world example](https://ashishjain1988.github.io/MAFDash/articles/Advanced_Example.html)

### Example dashboards from the vignette
Here are some example dashboards created using TCGA data:

- [Default dashboard using TCGA-LAML](https://mtandon09.github.io/MAFDashRPackage/examples/LAML.mafdash.html)
- [Customized dashboard using TCGA-UVM](https://mtandon09.github.io/MAFDashRPackage/examples/TCGA-UVM.custom.mafdash.html.MAFDash.html)
- [Arbitrary plots using `iris` dataset](https://mtandon09.github.io/MAFDashRPackage/examples/toy_dash.html.MAFDash.html)

#### Other notes
- This repo was born out of a Shiny app, [MAFWiz](https://github.com/mtandon09/mafwiz).  Instead of relying on a Shiny server, this dashboard was an attempt to try some of those things using client-side javascript functionality.
