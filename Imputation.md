### Data Cleaning

Imputation methods were required to correct eight datasets that were identified as having missing values. As demonstrated below, missingness plots were developed to ascertain this, with pink demonstrating the location of incomplete data. 

Tournament data had high percentages of missing values, shown through the following Missingness Maps.

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/MissingnessTournament.png)

League data represented lower percentages of missing values.

![](https://raw.githubusercontent.com/ACTL4001-T1-2022/github-showcase-page-tkgj-consulting/main/MissingnessLeague.png)

Multiple imputation methods were investigated and attempted. Some, such as the Amelia and MICE imputations, did not function well as they were not suited to the dataset, due to:
* Initial assumptions not aligning.
* They required character variables.
* Time taken to complete the imputation was inordinate. 

The KNN method was deemed most useful, due to appropriate run time and its examination of related values, meaning similar players, which aligns with the nature of the player data (Brownlee, 2020).

> Code used to assess the imputed variables is available [here](Imputation_Code). 
> The imputed data can be downloaded [here](TKGJ_Consulting_Data.xlsx). 
