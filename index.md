---
title       : Everybody Loves Shiny Oranges
subtitle    : Slidify Presentation for Data Products Final Project
author      : Michael Scully
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Let me tell you about Shiny Oranges

My Shiny Oranges app can be found here: 

https://viascully.shinyapps.io/DataProducts-ShinyApp/

and the code behind it can be found here:

https://github.com/viaScully/DataProducts-ShinyApp

and the Rmd code behind this presentation can be found here:

https://github.com/viaScully/ShinyOranges/tree/gh-pages


--- .class #id 

## It is a super simple app

This app that allows you to display a plot of age (in days) against trunk circumference (in mm) for orange trees.

Simply select one of the five trees measured, and the plot will update with the data for that tree.

The data used for this project is the 'Orange' data set in the 'datasets' package.

--- 

## It has everything

> 1. a Radio input
> 2. ui input that is used in server.R to filter the right data
> 3. plot for the selected tree that is generated as output that is rendered back in the ui
> 4. enough documentation that even a novice user can use this app
> 5. documentation that is right in the Shiny app itself

---

## Here's some R code that gets run upon Slidifying


```r
library(datasets)
data(Orange)
summary(Orange)
```

```
##  Tree       age         circumference  
##  3:7   Min.   : 118.0   Min.   : 30.0  
##  1:7   1st Qu.: 484.0   1st Qu.: 65.5  
##  5:7   Median :1004.0   Median :115.0  
##  2:7   Mean   : 922.1   Mean   :115.9  
##  4:7   3rd Qu.:1372.0   3rd Qu.:161.5  
##        Max.   :1582.0   Max.   :214.0
```

