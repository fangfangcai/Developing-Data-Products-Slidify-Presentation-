---
title       : Shiny app
subtitle    : Household Monthly Income Per Person Calculator
author      : Fangfang
job         : Learner
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---

## About the App

This app helps to calculate the Household Monthly Income Per Person. Household Monthly Income Per Person is the total gross household monthly income divided by the number of members living in the household.

Knowing the Household Monthly Income Per Person can help in the financial planning of a household.

--- .class #id 

## How the App works

1. Enter the monthly income of a member in the household under "income 1"

2. If there is another member in the household who is earning income, please enter the monthly income of that member in the household under "income 2" and so on. (Maximum of 6 incomes) You do not need to enter the income of members who do not have any income. You do not have to fill up all 6 incomes.

3. After entering the individual income of the household members who are earning, please enter the number of members living in the household.

4. Click on the submit button.

5. The Household Monthly Income Per Person will be calculated.

--- .class #id 

## Example

There are 5 members in a household.
Person 1 earns $3000 monthly.
Person 2 earns $2000 monthly.
Person 3 earns $1000 monthly.
Person 4 does not earn any income.
Person 5 does not earn any income.


```r
income_1 <- 3000
income_2 <- 2000
income_3 <- 1000
NumberOfMembers <- 5
Household_Monthly_Income_Per_Person <- (income_1 + income_2 + income_3)/NumberOfMembers
Household_Monthly_Income_Per_Person
```

```
## [1] 1200
```

The Household Monthly Income Per Person is $1200.

--- .class #id 

## Shiny App (run from shinyapps.io website)

<iframe src="http://fangfangcai.shinyapps.io/Shiny/">
</iframe>
