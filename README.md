
<!-- README.md is generated from README.Rmd. Please edit that file -->

# libminer

<!-- badges: start -->

[![R-CMD-check](https://github.com/R-icntay/libminer/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/R-icntay/libminer/actions/workflows/R-CMD-check.yaml)
<!-- badges: end -->

The goal of libminer is to show you the number of packages installed in
your computer and their respective sizes.

## Installation

You can install the development version of libminer from
[GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("R-icntay/libminer")
```

## Example

This is a basic example which shows you how to solve a common problem:

``` r
library(libminer)

## basic example code
lib_summary()
#>                                                                    Library
#> 1                                       C:/Program Files/R/R-4.3.0/library
#> 2                        C:/Users/homeuser/AppData/Local/R/win-library/4.3
#> 3 C:/Users/homeuser/AppData/Local/Temp/RtmpSEZglt/temp_libpath4b9c1b6a2b9e
#>   n_packages
#> 1         30
#> 2        146
#> 3          1

# Also calculate the sizes
lib_summary(sizes = TRUE)
#>                                                                    Library
#> 1                                       C:/Program Files/R/R-4.3.0/library
#> 2                        C:/Users/homeuser/AppData/Local/R/win-library/4.3
#> 3 C:/Users/homeuser/AppData/Local/Temp/RtmpSEZglt/temp_libpath4b9c1b6a2b9e
#>   n_packages  lib_size
#> 1         30  68685145
#> 2        146 222046885
#> 3          1     13362
```
