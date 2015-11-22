---
title       : Data product presentation
subtitle    : Course Project. Shiny Application and Reproducible Pitch
author      : Ignacio Reboredo
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
ext_widgets : {rCharts: [libraries/nvd3]}  
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---

## Exploratory analysis tool on mtcars dataset

This shiny app allows to conduct an exploratory analysis over a dataset of cars to explore the relationship between car’s transmission and miles per gallon (mpg) taking into consideration the potential influence of other variables

<div style='text-align: center;'>
    <img height='450' src='image1.png' />
</div>

--- .class #id 

## How to use it (options)

**The sidebar panel** allows to chose:
- The x axis variable you want to plot against the mpg (miles per galon)
- Include the linear regresion on the plot ("Regresions line and confidence interval" checkbox)
- If *Regesion line and confidence interval* checkbox is selected, the you can determine the confidence interval (70% to 97.5%) you want to show on the plot

<div style='text-align: center;'>
    <img height='350' src='image2.png' />
</div>

---

## How it looks like (plot tab)

- The Y axis represent "miles per galon"". X axis variable can be chosen on the sidebar menu
- Points in red represent automatic transmision cars. Blue points represent manual cars
- Particular implementation: mph vs hp, without confidence interval (R code to generate this plot can be seen on the .Rmd file included on the Github directory)

<img src="assets/fig/plot1-1.png" title="plot of chunk plot1" alt="plot of chunk plot1" style="display: block; margin: auto;" />


---

## How it looks like (plot tab)

- Regresion line is red for automatic cars and blue for manual ones
- Confidence interval is shown by a grey shadow
- Particular implementation: mph vs hp, with a confidence interval of 95% (R code to generate this plot can be seen on the .Rmd file included on the Github directory)

<img src="assets/fig/plot2-1.png" title="plot of chunk plot2" alt="plot of chunk plot2" style="display: block; margin: auto;" />

