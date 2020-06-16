Day 3 Practice
'''R
## packages
  library(tidyverse)
  library(dplyr)

## dataset
  data(mtcars)

## output cyl if value >= 6
  ## stores vals of cyl into list
    cyl.list <- mtcars$cyl
  ## outputs vals >= 6
    cyl.list[which(cyl.list >= 6)]

## make data frame named mtcars.2
  mtcars.2 <- data.frame(cyl.list[which(cyl.list == 8)])
## disply data set
  mtcars.2
  
## avg mpg of cars w cyl == 8
  ## stores vals of mpg into list
    mpg.list <- mtcars$mpg
  ## makes list of mpg w cyl == 8
    mpg.list.mod <- mpg.list[which(cyl.list == 8)]
  ## calculates mean
    mean(mpg.list.mod)
    '''
