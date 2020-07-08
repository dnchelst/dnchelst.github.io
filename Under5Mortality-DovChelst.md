Child Mortality Worldwide
===
author: Dov Chelst
transition: rotate
date: 2020-07-08


What are Mortality Rates?
===
<small>
- Mortality rates are one primary indicator of health.
- Mortality rates are collected annually for most regions throughout the world.
- I first encountered under-5 mortality rates (U5MR) in
[UNICEF](http://www.unicef.org/)'s annual 
[State of the World's Children](http://www.unicef.org/sowc/) report. 
([<font color="red">Donate</font>](http://www.supportunicef.org))
- U5MR measures the number of deaths below age 5 per 1,000 births.
- Many developed countries have rates below 10, indicating that less than 1% of children die by age 5.
- However, in some countries, rates exceed 100, indicating that over 10% of children die by age 5.
- Nevertheless, mortality rates have decreased overall between 1990 and 2018.
</small>

Why a U5MR App?
===
- Gather U5MR from [World Bank](http://data.worldbank.org/indicator/SH.DYN.MORT)  either directly or using 
[WDI](https://cran.r-project.org/web/packages/WDI/WDI.pdf) package from 1990
through 2018 (earlier data available).
- World U5MR: 1990=__93.2__,
2018=__38.6__
- Note the variation by region in 1990 and 2018 and the overall decrease for all measures over 29 years.

|Measure | Year.1990| Year.2018|
|:-------|---------:|---------:|
|Minimum |       6.3|       1.7|
|Q1      |      17.4|       6.9|
|Median  |      51.4|      17.6|
|Q3      |     126.8|      46.3|
|Maximum |     328.6|     121.5|
- App to provide further detail.

U5MR App Features
===
- Links: [u5mr-app](https://dnchelst.shinyapps.io/u5mr-app), 
[github](https://github.com/dnchelst/developingdata-dec2015)
- **Map** a single year to show variation throughout the world.
  - <small>Western Europe and Scandinavia show low mortality rates.</small>
  - <small>Portions of Africa show high mortality rates.</small>
- **Plot** a single country/region to show a general decreasing mortality rate 
over 29 years. (Selected year highlighted)
  - <small>Try out: South Korea, India, or Finland.</small>
- **Quick calculations** for the selected region and year. 
  - <small> _Rank_  is also shown with 1 as the lowest mortality rate.</small>
  - <small> _Percent change_  between 1990 and 2018 is also shown.</small>

Concluding Thoughts
===
- Extension 1: Additional data available from 1960.
- Extension 2: Multiple region selection, multiple trend lines
- Warning 1: Collection may be unreliable for some regions.
- Warning 2: Data may omit regions with changed boundaries or names.
- Warning 3: App generates errors but works: ("data not available for Taiwan...")
- R packages: WDI, leaflet, shiny, tidyverse
- **While the R packages are nice, the people who assembled U5MR data for over 
half a century deserve most of the credit.**
