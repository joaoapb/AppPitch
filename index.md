---
title       : Coursera Data Products
subtitle    : App Pitch
author      : João Augusto P. Batista
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Brazilian Labor Data

Brazilian Work and Employment Ministry releases microdata from all hiring and separations in the country, monthly. This data is available [here](ftp://ftp.mtps.gov.br/pdet/microdados/CAGED/).

--- .class #id 

## The Data

After being cleaned and grouped for this exercise, the data looks like this:


```r
db <- readRDS('assets/data/db.rds')
head(db)
```

```
##   Year State   mov  value
## 1 2009    11 Hires 125902
## 2 2009    12 Hires  23790
## 3 2009    13 Hires 163680
## 4 2009    14 Hires  13592
## 5 2009    15 Hires 254970
## 6 2009    16 Hires  20429
```


--- .class #id 

## What to see on the App
With the App hosted at [shinyapps.io](https://joaoapb.shinyapps.io/brazilian_labor_stats/) you can check the evolution by year and State of Hiring, Separations and the Net Hiring in Brazil, from 2009 to 2016, in a nice map. 

On the second tab, you can check the aggregated value for Brazil, as well as the year over year variation, along with a nice regression over the line.

--- .class #id 

## Other resources
For an example of a common analysis made with this data, check this [article](http://www.brazilgovnews.gov.br/news/2017/03/after-22-months-of-decline-brazil-creates-jobs-again) from March 2017.





