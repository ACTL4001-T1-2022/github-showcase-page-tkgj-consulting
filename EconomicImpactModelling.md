# Modelling of Economic Impact
---

> This section outlines how Rarita Football's revenues and expenses were forecasted through an analysis of economic trends and modelling of different types of revenue. The corresponding Excel workbook can be downloaded [here](Pre-Modelling_and_Economic_Analysis.xlsx).

### Economic and Population Trends
The limited years of economic data available for the regions of Rarita meant that medium-term sample means were taken to forecast the corresponding economic variables. It was assumed over the next 10 years that the economy would behave in line with these averages.



![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Table%20of%20Economic%20Trends.JPG)

### Forecasting Revenue and Expenses Over the Next 10 Years
Two processes of forecasting the cash flows were considered:
* A naive model which assumed per capital total revenue growth would follow some function of GDP per capita growth and that expenses would grow at its previous 5 year average.
* A comprehensive model that forecasted per capita commercial, matchday and broadcast revenue seperately and that expenses would grow at its previous 5 year average.
>Both models assumed that the populations of each region of Rarita would continue to grow at their 10 year average growth rates. The tolerance for these models were p-values of 0.1 or less when considering statistical significance, which both models comfortably passed.
#### Naive Model
The naive model utilised simple linear regression with the dependent variable being per capital total revenue and the sole independent variable being GDP per capita. The justification for this was that as an economy grows, incomes will grow and will allow individuals to spend more money on leisure related goods, including those related to Raritan football. GDP growth was assumed to grow at a constant 3.94% per year as outlined aboved.

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Total%20Revenue%20and%20GDP%20per%20Capita%20Model.JPG)

Expense growth was assumed to grow at its 5 year average of 6.9%. The above results were combined to first forecast GDP per capita from 2021-2030 and then substitute these values into the simple linear regression model to forecast total revenue per capita. Total expenses per capita were also forecasted and both these figures were then multiplied by the projected population for that particular year to get total revenue and expenses.

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Naive%20Model%20Summary.JPG)

> A more detailed breakdown can be found [here](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Naive%20Model%20Forecast.jpg)

As seen above, the projected net present value of all future cash flows is a profit of 6.43 billion doubloons.

#### Comprehensive Model
The comprehensive model utilised several simple linear regression models to assist in forecasting per capita matchday and commercial revenue. It also considered Rarita's football rank as a factor affecting revenue. Broadcast revenue was assumed to grow in line with its previous 5 year average of 4.2% annually and expense growth was once again assumed to remain at 6.9% per year. 

The strong relationship between social media following and a nation's football rank was explored through a simple linear regression model. The intuition behind this was that stronger performance would create more fans who would likely use social media (especially younger generations).

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Social%20Media%20and%20Football%20Rank%20Model.JPG)

The above model was utilised to predict commercial revenue by then regressing per capita commercial revenue on social media following. The intuition was that one would expect that a strong online following would entice companies to sponsor Raritan football and also experience a rise in merchandise sales.

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Per%20Capita%20Commercial%20Revenue%20and%20Social%20Media%20Model.JPG)

>Using the projected Raritan football ranking of 8.2, commercial revenue was able to be forecasted (see below).

Per capita matchday revenue (revenue from ticket sales) was also assumed to be influenced by rank, as a stronger football nation is likely to have a higher quality league and a more attractive playstyle with popular players competing. 

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Per%20Capita%20Matchday%20Revenue%20and%20Football%20Rank%20Model.JPG)

>Using the projected Raritan football ranking of 8.2, matchday revenue was able to be forecasted (see below).

These projections were combined alongside the assumptions regarding broadcast and expense growth outlined above to forecast profit (by multiplying per capita revenues/expenses by the same projected populations from the naive model)

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Comprehensive%20Model%20Summary.JPG)

> A more detailed breakdown of [commercial](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Comprehensive%20Model%20Commercial%20Revenue%20Forecast.jpg), [matchday](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Comprehensive%20Model%20Matchday%20Revenue%20Forecast.jpg) and [broadcast](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/Comprehensive%20Model%20Broadcast%20Revenue%20Forecast.jpg) revenues and a total revenue/expense breakdown can be found [here](https://github.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/blob/main/Comprehensive%20Model%20Forecast.jpg)
