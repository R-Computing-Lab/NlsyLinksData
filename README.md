NlsyLinks
================

NlsyLinks is a free downloadable R package to facilitate Behavior Genetic and Family Studies research using the NLSY samples (the National Longitudinal Survey of Youth).  These samples are based on a cross-generational longitudinal nationally representative sample of over 30,000 participants followed for up to 35 years.  There are almost 50,000 pairwise kinship links.

Get started at [here](http://www.bls.gov/nls/) the NLSY and [here](http://nlsy-links.github.io/NlsyLinks/) for the NlsyLinks package.

Installing
--------------------------

The *release* version of `NlsyLinks` can be installed from [CRAN](https://cran.r-project.org/package=NlsyLinks).

```r
install.packages("NlsyLinks")
```

The latest *development* version of `NlsyLinks` can be installed from [GitHub](https://github.com/nlsy-links/NlsyLinks/) after installing the `remotes` package.

```r
install.packages("remotes")
remotes::install_github(repo="nlsy-links/NlsyLinks")
```

Obtaining the Links
--------------------------

There are roughly three versions of the links:

1. The *release* versions are bundled in the `NlsyLinks` package and updated once or twice a year during development.
1. The *pre-release* versions are downloadable from our [team's website](http://nlsy-links.github.io/NlsyLinks/) and updated several times a month during development.  Formats include R, SAS, and plain-text CSV.
1. The *development* versions are downloadable from our [determination repo](https://github.com/nlsy-links/nlsy-links-determination-2017) updated several times a day during development.

Locations for Help and Development
--------------------------

This repository contains the code used in the [NlsyLinks](https://cran.r-project.org/package=NlsyLinks) R package.  For additional information about the package and using it in NLSY research, please see <http://nlsy-links.github.io/NlsyLinks>.

[This GitHub repository](https://github.com/nlsy-links/NlsyLinksStaging) is our primary way of managing, tracking, and build-checking versions of the source code.  (We're no longer using our [R-Forge site](https://r-forge.r-project.org/projects/nlsylinks/).)  The stable releases (intended for most researchers) is available on the package's [CRAN site](https://cran.r-project.org/package=NlsyLinks).

We recently moved the forums to <https://groups.google.com/forum/#!forum/nlsy-links>.  Previous conversations are available at our old [R-Forge](https://r-forge.r-project.org/forum/?group_id=1330) and [Disqus](https://disqus.com/home/forum/nlsylinks/) sites.

Publication
--------------------------

Please see [research-publications](http://nlsy-links.github.io/NlsyLinks/research-publications.html) for a list of the 70+ publications arising from the kinship links.  An overview is available at:

Joseph Lee Rodgers, William H. Beasley, David E. Bard, Kelly M. Meredith, Michael D. Hunter, Amber B. Johnson, Maury Buster, Chengchang Li, Kim O. May, S. Mason Garrison, Warren B. Miller, Edwin van den Oord, and David C. Rowe (2016). *Behavior Genetics, 46*. [https://doi.org/10.1007/s10519-016-9785-3](https://doi.org/10.1007/s10519-016-9785-3).

>The National Longitudinal Survey of Youth datasets (NLSY79; NLSY-Children/Young Adults; NLSY97) have extensive family pedigree information contained within them. These data sources are based on probability sampling, a longitudinal design, and a cross-generational and within-family data structure, with hundreds of phenotypes relevant to behavior genetic (BG) researchers, as well as to other developmental and family researchers. These datasets provide a unique and powerful source of information for BG researchers. But much of the information required for biometrical modeling has been hidden, and has required substantial programming effort to uncover—until recently. Our research team has spent over 20 years developing kinship links to genetically inform biometrical modeling. In the most recent release of kinship links from two of the NLSY datasets, the direct kinship indicators included in the 2006 surveys allowed successful and unambiguous linking of over 94 % of the potential pairs. In this paper, we provide details for research teams interested in using the NLSY data portfolio to conduct BG (and other family-oriented) research.

Thanks to Funders
--------------------------

The current work on the NLSY Kinship links has been supported by NIH Grant R01-HD065865 ([Joe Rodgers](http://www.vanderbilt.edu/psychological_sciences/bio/joe-rodgers), PI).

Status
--------------------------

| [GitHub](https://github.com/nlsy-links/NlsyLinks) | [Travis-CI](https://travis-ci.org/nlsy-links/NlsyLinks/builds) | [AppVeyor](https://ci.appveyor.com/project/wibeasley/nlsylinks/history) |  [Coveralls](https://coveralls.io/r/nlsy-links/NlsyLinks) |
| :----- | :---------------------------: | :------------: | :-------: |
| [Master](https://github.com/nlsy-links/NlsyLinks/tree/master) |  [![Travis-CI Build Status](https://travis-ci.org/nlsy-links/NlsyLinks.png?branch=master)](https://travis-ci.org/nlsy-links/NlsyLinks) | [![Build status](https://ci.appveyor.com/api/projects/status/fo1oeqn9734dhhmu/branch/master?svg=true)](https://ci.appveyor.com/project/wibeasley/nlsylinks/branch/master) | [![Coverage Status](https://coveralls.io/repos/nlsy-links/NlsyLinks/badge.svg?branch=master)](https://coveralls.io/r/nlsy-links/NlsyLinks?branch=master) |
| [Dev](https://github.com/nlsy-links/NlsyLinks/tree/dev) | [![Travis-CI Build Status](https://travis-ci.org/nlsy-links/NlsyLinks.png?branch=dev)](https://travis-ci.org/nlsy-links/NlsyLinks) | [![Build status](https://ci.appveyor.com/api/projects/status/fo1oeqn9734dhhmu/branch/dev?svg=true)](https://ci.appveyor.com/project/wibeasley/nlsylinks/branch/dev) | [![Coverage Status](https://coveralls.io/repos/nlsy-links/NlsyLinks/badge.svg?branch=dev)](https://coveralls.io/r/nlsy-links/NlsyLinks?branch=dev) |
| | *Ubuntu LTS* | *Windows Server* |  *Travis Code Coverage* |

| [CRAN](https://cran.r-project.org/) | [Version](https://cran.r-project.org/package=NlsyLinks) | [Rate](http://cranlogs.r-pkg.org/) | [Zenodo](https://zenodo.org/search?ln=en&p=nlsylinks) |
|  :---- | :----: | :----: | :----: |
| [Latest](https://cran.r-project.org/package=NlsyLinks) | [![CRAN_Status_Badge](http://www.r-pkg.org/badges/version/NlsyLinks)](https://cran.r-project.org/package=NlsyLinks) | ![CRANPace](http://cranlogs.r-pkg.org/badges/NlsyLinks) | [![DOI](https://zenodo.org/badge/doi/10.5281/zenodo.49941.svg)](http://dx.doi.org/10.5281/zenodo.49941) |
|   | *Latest CRAN version* | *CRAN Downloads* | *Independently-hosted Archive* |
