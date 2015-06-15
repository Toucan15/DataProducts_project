---
title       : Temperature change with elevation
subtitle    : for hikers and mountain travelers
author      : toucan15
job         : coursera 09 data products
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## Temperature Change Calculator

Air temperature changes with elevation.

In general, the temperature decreases 3.5 degrees F for every 1000 feet in elevation gain.

If people don't plan ahead when hiking or traveling in the mountains they could be exposed to cold conditions and possibly hypothermia.

---.class #id  

## Intended Users

Hikers and mountain travelers can use this app to anticipate temperature changes due to elevation and to therefore be better prepared for cooler conditions at higher elevations. 

The app can also be used to predict warmer temps at lower elevations although descending into warmer conditions is usually not as unexpected as ascending into cold conditions.

---.class #id

## Here's How it Works

Typical temperature change is 3.5 degrees Fahrenheit for every 1000 feet in elevation gain. To calculate the expected temperature change the app subtracts ending from starting elevation, divides the result by 1000 feet, then multiplies by 3.5 degrees.

For example, let's say you start in Denver at about 5500 feet elevation and drive to the top of Mt Evans at 14200 feet. It's a warm day, 70 degrees F when you start. 


```r
x <- ((5500-14200)/1000)*3.5
```

The expected temperature change is

```
## [1] -30.45
```

In other words, it will be close to 30 degrees colder at 14200 feet than at 5500 feet so you should bring enough layers to be comfortable at 40 degrees.

---.class #id

## Ease of use

The app is easy to use and requires just two inputs: elevation at the start and expected elevation at the destination.

Then the app calculates the expected change in temperature. If the result is negative, the temperature is expected to get colder. If the result is positive the temperature is expected to get warmer.

This app can be used for elevations up to 20,000 feet. Above that level are the tallest mountains on earth and climbing these peaks is much difficult and technical. This app is intended for more casual use and thus does not include the highest mountains. 

---.class #id
