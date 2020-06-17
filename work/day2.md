practice_day4

#*test

#'test

```
# loading
data("iris")

# installed packages
library(tidyverse)
library(dplyr)

# median, min, max iris
max(iris$Petal.Width)
min(iris$Petal.Width)
median(iris$Petal.Width)

petal_width_moments <- function(x) {
  iris_max <- max(x) 
  iris_min <- min(x) 
  iris_median <- median(x)
  output_moments <- c(iris_max, iris_min, iris_median)
  return(output_moments)
}

petal_width_moments(iris$Petal.Width)

# std.err <- function(x){
#   n <- length(x)
#   stnd_dev <- sd(x)
#   std_error <- stnd_dev / sqrt(n)
#   return(std_error)
# }
# 
# std.err(iris$Petal.Width)



# loading
data("Orange")

# installed packages
library(tidyverse)
library(dplyr)

# max circumference
max_cir <- max(Orange$circumference, na.rm = TRUE)
max_cir
  
# min circumference
min_cir <- min(Orange$circumference, na.rm = TRUE)
min_cir

# median circumference
median_cir <- median(Orange$circumference, na.rm = TRUE)
median_cir

orange_cir_sum <- summary(Orange$circumference)
summary(Orange$circumference)[c(1,3,6)]


```
