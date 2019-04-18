
<!-- README.md is generated from README.Rmd. Please edit that file -->
[![Build Status](https://travis-ci.org/PublicHealthEngland/PHEindicatormethods.svg?branch=master)](https://travis-ci.org/PublicHealthEngland/PHEindicatormethods?branch=master)

[![Coverage Status](https://coveralls.io/repos/github/PublicHealthEngland/PHEindicatormethods/badge.svg?branch=master)](https://coveralls.io/github/PublicHealthEngland/PHEindicatormethods?branch=master)

PHEindicatormethods
===================

This is an R package to support analysts in the execution of statistical methods approved for use in the production of PHE indicators such as those presented via Fingertips. It provides functions for the generation of Proportions, Rates, DSRs, ISRs, SMRs, Means, Life Expectancy and Slope Index of Inequaltiy including confidence intervals for these statistics, and a function for assigning data to quantiles.

Any feedback would be appreciated and can be provided using the Issues section of the GitHub repository <https://github.com/PublicHealthEngland/PHEindicatormethods>, or by emailing <PHDS@phe.gov.uk>

<br/> <br/>

Installation
------------

#### Install from CRAN

Install the latest release version of PHEindicatormethods directly from CRAN with:

``` r
install.packages("PHEindicatormethods")
```

#### Install a development version from GitHub using devtools

You can install a development version of PHEindicatormethods from GitHub with:

``` r
if (!require(remotes)) install.packages("remotes")

remotes::install_github("PublicHealthEngland/PHEindicatormethods",
                         build_vignettes = TRUE,
                         dependencies = TRUE,
                         build_opts = c("--no-resave-data"))
```

#### Install a development version from zip

Download the PHEindicatormethods repository from GitHub <https://github.com/PublicHealthEngland/PHEindicatormethods> and either build from source or do:

``` r
if (!require(devtools)) install.packages("devtools")

source <- devtools:::source_pkg("C:/path/to/PHEindicatormethods-master")
devtools::install(source)
```

<br/> <br/>

Package Versioning
------------------

Following installation of this package, type 'packageVersion("PHEindicatormethods")' in the R console to show the package version. If it is suffixed with a 9000 number then you are using an unapproved development version.

Released versions of this package will have version numbers consisting of three parts:

major.minor.patch

In-development versions of this package will have a fourth component, the development version number, which will increment from 9000.

See <http://r-pkgs.had.co.nz/description.html> for further information on package versioning

<br/> <br/>

Package Contents
----------------

The package contains the following functions, datasets and vignettes - see individual item documentation for full details

**Functions:**

-   phe\_dsr
-   phe\_isr
-   phe\_mean
-   phe\_proportion
-   phe\_quantile
-   phe\_rate
-   phe\_smr
-   phe\_quantile
-   phe\_life\_expectancy
-   phe\_sii

**Datasets:**

-   esp2013
-   LE\_data (for use with SII vignette)
-   DSR\_data (for use with SII vignette)
-   prevalence\_data (for use with SII vignette)

**Vignettes:**

-   Vignette to introduce the package functions included in the original package release
-   Vignette for calculating DSRs for multiple geographies and time periods
-   Vignette showing worked examples of the phe\_sii function

(type 'browseVignettes("PHEindicatormethods")' to view in HTML)
