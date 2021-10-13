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

``` r
cases = readr::read_csv(gsub("[ \n]", "",
  "https://urmc-bst.github.io/
   bst430-fall2021-site/hw_lab_instruction/lab06-covid-times/data/us-states.csv"))
```

    ## Rows: 32318 Columns: 9

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr  (2): geoid, state
    ## dbl  (6): cases, cases_avg, cases_avg_per_100k, deaths, deaths_avg, deaths_a...
    ## date (1): date

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

Add exercise headings, chunks, etc, as needed.

## Ex7

``` r
row_var = function(matrix, na_rm = FALSE) {
  apply(matrix, 1, var, na.rm = na_rm)
}
```
