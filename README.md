# AutoStock-Population
This report will investigate the relationship between the high crime rate and the automotive industry.

   Detroit is a city that is well known for its struggle with high crime rates, a crime rate often associated with a variety of problems that have plagued the city since the downturn of the auto industry and industrial restructuring. The Motor City is synonymous with the American automotive industry, an industry that dominated the city's culture and economy. This report will investigate the relationship between the high crime rate and the automotive industry.
   Two datasets were used in this report, Detroit Major Crimes 2011-2014 dataset by the City of Detroit and Huge Stock Market Dataset both stored as CSVs. The first dataset reported major crime offenses from Jan 1, 2011, through Dec 31, 2014, for the City of Detroit. The second contained historical stock market data for the three largest employers in Detroit: Ford, General Motors, and Chrysler. This dataset was relatively consistent but also needed some tidying as a result of NA values and blank rows.
   To analyze the data I limited the sample size to 2014 and averaged the stock closing price trends across the three employers while also normalizing the data using an R-Log transformation to help with comparison on the graph. I then joined the average closing price trends with the crime counts per day and displayed them on a graph. The graph allowed us to visualize trends in the two variables and suggested that the correlation may be nonlinear, ultimately informing our decision to use a Spearman’s test instead of a Pearson. The graph itself however was inconclusive and didn’t provide insight into the existence of a correlation, while there did seem to be a relationship towards the end of the graph. The Spearman test was conducted with a null hypothesis of no correlation and an alternative hypothesis of a correlation. The result was a p-value of 0.2268 and a sample estimate of a rho being -0.0827644. These results mean we fail to reject the null hypothesis at a 5% significance level.
    Based on these results we can not conclude that there is a correlation between employer performance and crime rates in Detroit. This is because our hypothesis testing provided no statistical evidence of covariation between the two variables. While economic factors may play a role in crime rates in Detroit, this report provides no conclusive evidence toward that effect.
 
 
Works Cited:

City of Detroit. (2016, September 19). Detroit Major Crimes 2011-2014 - dataset by Detroit. data. world. Retrieved April 9, 2023, from https://data.world/detroit/detroit-major-crimes-2011-2014
Marjanovic, B. (2017, November 16). Huge stock market dataset. Kaggle. Retrieved April 9, 2023, from https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs
