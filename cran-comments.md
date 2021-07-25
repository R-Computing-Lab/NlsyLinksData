Description
-----------------------------------------------

This submission revival of a package archived in April.

Regarding package size ("the installed size is 6.0Mb"): A few years ago Kurt asked, "Would it be possible to put some of the data sets into a separate package which changes less frequently than code and docs?" I'll gladly defer to your judgment and recommendations, but I see two reasons to retain a united package.  First, our primary target audience is Behavior Genetics researchers, who typically are much less familiar with R than other fields.  There have been at least 3 BG researchers who have requested SAS data files, because they weren't even comfortable reading vanilla CSV files into SAS.  I'd like to avoid another step/package for them to consider, even if the dataset-only package was a dependency.  Second, the datasets change every few years because the NLSY's three current cohorts are surveyed every two years.  This will be only the [third CRAN submission since Dec 2013](https://cran.rstudio.com/src/contrib/Archive/NlsyLinks/), and most of those changes [were to stay current updated CRAN policies](https://cran.rstudio.com/web/packages/NlsyLinks/NEWS).  The dataset-package would have needed to change too, and therefore increase the demands on CRAN maintainers (because both packages might required updates).

However, I'm happy to split this package if that's what you feel is best for CRAN and R users.  -Will Beasley

Test environments
-----------------------------------------------

1. Local Ubuntu, R 4.1.0 patched
1. Local Win8, R 4.1.0 patched
1. Local Win10, R 4.1.0 patched
1. R-hub
    1. [Ubuntu Linux 20.04 LTS, R-release, GCC](https://builder.r-hub.io/status/NlsyLinks_2.0.9.9001.tar.gz-e487560c78d7460cba4f7fa2ffef8c6c)
    1. [Fedora Linux, R-devel, clang, gfortran](https://builder.r-hub.io/status/NlsyLinks_2.0.9.9001.tar.gz-25cb9276478f4b4db3a8b1ebc6dc8b80)
    1. [Windows Server](https://builder.r-hub.io/status/REDCapR_1.0.0.tar.gz-b5b0cb95fb4746f9b354071b89caaafa)
1. [win-builder](https://win-builder.r-project.org/y4W36ZKoyyc8/00check.log), development version.
1. [GiHub Actions](https://github.com/OuhscBbmc/REDCapR/actions), Ubuntu 20.04 LTS

R CMD check results
-----------------------------------------------

* No ERRORs or WARNINGs on any builds.
* Two notable NOTEs:
    1. This is a new submission of a package that is currently archived.
    2. The package size has a few large data files; the data size is around 4Mb.  I believe the size is justified because it drastically reduces the code needed for the package user to start incorporating their outcomes on to the larger familial framework we've build.  (One of the package's cornerstones is how we've linked the 24,000 participants within the 5,160 extended families.)
        a. The (uncompressed) CSV is needed for an important example how to incorporate the CSVs downloaded from the NLSY database.  I've used only the necessary columns.
        b. The compressed RDA files have important participant data the allows the package user to incorporate
* No other unexplainable NOTEs.  The Ubuntu R-hub build complains about some images in a vignette, but I think that's something specific to that test environment, and not to the package.  The other builds (including the other two R-hub builds) don't throw the same warning.

Downstream dependencies
-----------------------------------------------
No other packages depend/import this one.
