---
title       : The Safe Gatsby
subtitle    : The Shiny App for estimating the Stopping Distance of 1920s Oldtimers
author      : JimboB
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Motivation 

Driving an oldtimer from the 1920s can be a perilous endeavor. Differences in technology between the 1920s and the 21. century make it difficult for people who are used to modern cars to estimate the necessary stopping distance of their oldtimer.
__The__ __Safe__ __Gatsby__ provides you with an estimate of the stopping distance given the velocity of yout oldtimer based on a statistical model.

![alt text](assets/img/car.jpg)

--- .class #id 

## Dataset

The dataset used for the model consists of 50 observations of speed and stopping distance of 1920s cars. It is part of the R package _datasets_ and is free to use.

```r
library(datasets)
data("cars")
summary(cars)
```

```
##      speed           dist       
##  Min.   : 4.0   Min.   :  2.00  
##  1st Qu.:12.0   1st Qu.: 26.00  
##  Median :15.0   Median : 36.00  
##  Mean   :15.4   Mean   : 42.98  
##  3rd Qu.:19.0   3rd Qu.: 56.00  
##  Max.   :25.0   Max.   :120.00
```

---

## The Model

$distance = speed + speed^2 $

![plot of chunk unnamed-chunk-2](assets/fig/unnamed-chunk-2-1.png) 


---

## Try it!

URL: [https://jimbob.shinyapps.io/TheSafeGatsby](https://jimbob.shinyapps.io/TheSafeGatsby)

Just enter the speed in Miles per Hour and calculate the estimated stopping distance!

---



