# **QuantQC: nPOP sample preparation evaluation pipline**



* [nPOP sample preparation Website](https://scp.slavovlab.net/nPOP) &nbsp; | &nbsp; [Download data from origninal publication](https://scp.slavovlab.net/Leduc_et_al_2022) | &nbsp; [Download data from protocol](https://scp.slavovlab.net/Leduc_et_al_2022)

* [Preprint of Protocol](https://scp.slavovlab.net/Leduc_et_al_2022)

* [Preprint Original Article](https://www.biorxiv.org/content/10.1101/2021.11.03.467007v2) &nbsp; | &nbsp; [*Genome Biology* Article](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-022-02817-5)


&nbsp;

![alt text](https://github.com/Andrew-Leduc/QuantQC/blob/main/img/head.png?raw=true)


### Requirements

This application has been tested on R >= 3.5.0, OSX 10.14 / Windows 7/8/10. R can be downloaded from the main [R Project page](https://www.r-project.org/) or downloaded with the [RStudio Application](https://www.rstudio.com/products/rstudio/download/).

There are three packages that are not installed by default. They are not needed for all tasks, it will let you know if you need them if you'd rather not install.

  1. [Seurat](https://satijalab.org/seurat/articles/install.html)
  2. [XGboost](https://xgboost.readthedocs.io/en/latest/R-package/index.html)
  3. [DIANN r package](https://github.com/vdemichev/diann-rpackage)

To install the QuantQC package, run (you may need to install devtools first):

```
devtools::install_github("https://github.com/SlavovLab/QuantQC")
library(QuantQC)
```


------------

## Reproducing the data analysis


1. Download all the data reports from the "search" section of MassIVE [MSV000093494](https://massive.ucsd.edu/ProteoSAFe/dataset.jsp?task=ac44b779d8a04ca285a263616796c3b8).

2. Download the "AnalysisFromProtocol" folder from the [QuantQC](https://github.com/Andrew-Leduc/QuantQC) Github page. In the R script "Analysis.R", change the path names for the relevant meta data files. There are two types. The linker file which connects the file names from the MS runs to the wells of the plate they were run from, and the cellenONE cell sorting files. These files are origninally named XXX_isolated.xls and are auto generated by the cellenONE in the folder created when the user performs cell sorting to the glass slide.

3. Run the Analysis.R script line by line following the comments in the script.



## About the project

<!--
QuantQC is an R package

-->
The manuscript is freely available on bioRxiv: [Leduc et al., 2023](https://www.biorxiv.org/content/10.1101/2021.11.03.467007v2).

For more information, contact [Slavov Laboratory](https://slavovlab.net) or directly [Andrew Leduc](https://coe.northeastern.edu/people/slavov-nikolai/)

### License

The QuantQC code is distributed by an [MIT license](https://github.com/SlavovLab/DO-MS/blob/master/LICENSE).

### Contributing

Please feel free to contribute to this project by opening an issue or pull request.

<!--
### Data
All data used for the manuscript is available on [UCSD's MassIVE Repository](https://massive.ucsd.edu/ProteoSAFe/dataset.jsp?task=ed5a1ab37dc34985bbedbf3d9a945535)
-->

<!--
### Figures/Analysis
Scripts for the figures in the DART-ID manuscript are available in a separate GitHub repository, [https://github.com/SlavovLab/DART-ID_2018](https://github.com/SlavovLab/DART-ID_2018)
-->

-------------

## Help!

For any bugs, questions, or feature requests,
please use the [GitHub issue system](https://github.com/SlavovLab/plexDIA/issues) to contact the developers.
