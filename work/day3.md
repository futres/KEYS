r training day 3

```

## data sets
data("HairEyeColor")

## packages
library(tidyverse)
library(dplyr)

## function
  ## avg function
  avg <- function(x) {
    avg_mean <- mean(x)
    return(avg_mean)
  }
  
  ## standard deviation error function
  sd_err <- function(y){
    n <- length(y)
    stand_dev <- sd(y)
    stand_err <- stand_dev / sqrt(n)
    return(stand_err)
  }

## function output
avg(Orange$age)
avg(Orange$circumference)
sd_err(Orange$age)
sd_err(Orange$circumference)

```
