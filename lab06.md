Lab 06 - Covid Times
================
Insert your names here
Insert date here

# Lab 06

## Load packages and data

``` r
library(reshape2)
library(tidyverse)
library(lubridate)
```

Add exercise headings, chunks, etc, as needed.

## Ex7

``` r
row_var = function(matrix, na_rm = FALSE) {
  apply(matrix, 1, var, na.rm = na_rm)
}
```
