
<!-- README.md is generated from README.Rmd. Please edit that file -->

# yyyymm

<!-- badges: start -->

[![Lifecycle:
stable](https://img.shields.io/badge/lifecycle-stable-brightgreen.svg)](https://www.tidyverse.org/lifecycle/#stable)
[![Codecov test
coverage](https://codecov.io/gh/jbkunst/yyyymm/branch/master/graph/badge.svg)](https://codecov.io/gh/jbkunst/yyyymm/branch/master)
[![R build
status](https://github.com/jbkunst/yyyymm/workflows/R-CMD-check/badge.svg)](https://github.com/jbkunst/yyyymm/actions?workflow=R-CMD-check)
<!-- badges: end -->

The goal of `yyyymm::` is to make life easier with period format.

## Installation

``` r
source("https://install-github.me/jbkunst/yyyymm")
```

## Some Examples

This is a basic example which shows you how to solve a common problem:

``` r
library(yyyymm)
ym_to_date(ym = c(200902, 201912), day = 1)
#> [1] "2009-02-01" "2019-12-01"
```

Get month differences:

``` r
ym_diff(ym = c(200902, 201912), ym2 = c(200901, 201712))
#> [1]  1 24


ym_add_months(c(200902, 201912), months = c(1, -12))
#> [1] 200903 201812
```

## Code of Conduct

Please note that `yyyymm::` project is released with a [Contributor Code
of Conduct](CODE_OF_CONDUCT.md). By contributing to this project, you
agree to abide by its terms.
