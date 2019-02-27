Practice Github Assignment
================

Load the packages
-----------------

Loading the R packages

``` r
library(readxl)     # load readxl, for reading Excel files
library(tidyverse)  # load tidyverse, for working with datasets
```

    ## -- Attaching packages ------------------------------ tidyverse 1.2.1 --

    ## v ggplot2 3.1.0       v purrr   0.3.0  
    ## v tibble  2.0.1       v dplyr   0.8.0.1
    ## v tidyr   0.8.2       v stringr 1.4.0  
    ## v readr   1.3.1       v forcats 0.4.0

    ## -- Conflicts --------------------------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

Read the Data
-------------

Reading data from excel file (included) and confirming it transferred

``` r
finches <- read_excel("finches_data.xlsx")
finches
```

    ## # A tibble: 100 x 12
    ##     band species sex   first_adult_year last_year outcome weight  wing
    ##    <dbl> <chr>   <chr>            <dbl>     <dbl> <chr>    <dbl> <dbl>
    ##  1     9 Geospi~ unkn~             1975      1977 died      14.5  67  
    ##  2    12 Geospi~ fema~             1975      1977 died      13.5  66  
    ##  3   276 Geospi~ unkn~             1976      1977 died      16.4  64.2
    ##  4   278 Geospi~ unkn~             1976      1977 died      18.5  67.2
    ##  5   283 Geospi~ male              1976      1977 died      17.4  70.2
    ##  6   288 Geospi~ unkn~             1976      1977 died      16.3  71.2
    ##  7   293 Geospi~ unkn~             1976      1977 died      15.7  67.2
    ##  8   294 Geospi~ unkn~             1976      1977 died      16.8  68.2
    ##  9   298 Geospi~ male              1976      1977 died      15.5  68.2
    ## 10   307 Geospi~ male              1975      1977 died      17.5  70  
    ## # ... with 90 more rows, and 4 more variables: tarsus <dbl>,
    ## #   beak_length <dbl>, beak_depth <dbl>, beak_width <dbl>
