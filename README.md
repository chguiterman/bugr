# **bugr**

------
Detection and analysis of insect defoliation signals in tree rings
------

[![Coverage Status](https://coveralls.io/repos/github/chguiterman/bugr/badge.svg?branch=master)](https://coveralls.io/github/chguiterman/bugr?branch=master)

### Some basics

`bugr` requires two independent datasets: 
* Host-tree series, as standardized ring widths. 
* A non-host standardized tree-ring chronology.
These datasets can be created in ARSTAN or using the `detrend()` function in the `dplR` library. Once read into R, the data can be passed to `bugr` functions. They must share the formatting of `rwl` objects in `dplR`.

Data are provided in this package to demonstrate some of the utilities of `bugr`, courtesy of Dr. Ann Lynch. 
Here, we can read in Douglas-fir host series from the East Fork site in the Jemez Mountains, `ef`.

```{r, eval = TRUE}
library(bugr)

data(ef)

head(ef)
```
