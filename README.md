# Excel-for-Everyone-Data-Analysis-Fundamentals
edX.org

## Course: Excel for Everyone: Data Analysis Fundamentals ##
Designed for more experienced Excel users to explore the methods to extract knowledge from large amounts of data.
## Institution: University of British Columbia ##
## Case Study: Analyzing Stock Market Data ##
## Level: Intermediate ##
## Date of completion: 2022-01-22 ##

# Analyzing Stock Market Data #

The case study makes use of a stock market data set with a six-month sample of trading activity for over 500 public businesses from 2017.
In addition to the close price and trading volume, the stock market data also includes the daily open high and low values for the equities.

Two tasks are involved in this project:
1. To design a smart **dashboard** so that stakeholders can see trends and changes. I selected graphics that I believed combined a complete grasp of the information in an interactive way.
2. Perform **data analysis** to better understand the data and explore it for additional prediction analysis. I will utilize  Descriptive Statistics, Histograms, Sampling, and Correlation from Data Analysis.

As it was gathered from the course sources, the data has already been sorted and there aren't any missing values. The Table can be found in the Stock Data spreadsheet.

### StockDashboard Spreadsheet ###

1. This type of line graph, which is used to examine trends and changes over time, doesn't reveal which companies are being followed, therefore it isn't very instructive in this situation. The Symbol slicer is the only source of information about the companies.
2. Open & Close Points, High & Low Price per Company - The clustered bars and stacked column graphs are used to compare two categories for each graph, and they also display the companies that were selected. Though they lack the info on dates, those are indicated in the Date slicer.

Together all graph complement what the other is lacking.

### StockStats Spreadsheet ###

#### *Descriptive Statistics* on the Open and Close Points, High and Low Prices, and Volume ####

1. Open and Close Points, High and Low Prices Standard Deviation shows a dispersion of ~119 from mean ~96, showing a lower deviation
   1. Kurtosis = 87, Skewness = 7.8 meaning distribution is too peaked (acceptable values for positive kurtosis according to various literature range from +2 to +10, and for 
      positive skewness varies from +0.5 to +3, but never exceeds these values)
2. Volume Standard Error  Standard Deviation shows a dispersion of 7,851,970 from a mean of 4,090,859 showing a higher deviation
   1. Kurtosis  = 155, Skewness = 9.5 meaning distribution is too peaked (acceptable values for positive kurtosis according to various literature ranges from +2 to +10, and for 
      positive skewness varies from +0.5 to +3, but never exceeds these values)

### StockAnalysis Spreadsheet ###

#### Data Analysis on the Open and Close Points, High and Low Prices, and Volume ####

*1. Sampling*
    *Random Sampling* for Open Points, High and Low Prices – Number of randomly selected values from the population – 20 for each
    *Systematic Random Sample* for Close Points and Volume – Random starting point (Row 22) and a sample interval of 20 with which the sample group is selected from the target 
     population, giving 3,128 samples for each
*2. Histogram*
    1. To show the frequency in bins for the Open and Close Points, High and Low Prices starting from 500, to 2,000, as the max values ~ 1,900
       Most frequent values under the range of value from 0 - 500, total data points come greater than 61,880 for these 4 columns
    2. To show the frequency in bins for the Values starting from 100,000 to 300,000,000 as max values = 268,336,455
       Most frequent values under the range of value from 100,001 – 100,000,000, total data points come = 62,489
*3. Correlation*
    To determine the relationship between the columns Open and Close Points, High and Low Prices, and Values

-------------|---------|---------|---------|---------|---------|
Correlation  |   Open  |   High  |   Low   |  Close  |  Volume | 
-------------|---------|---------|---------|---------|---------|	
Open	     |   1,00  | 	 |	   |         |         |
-------------|---------|---------|---------|---------|---------|
High	     |   1,00  |   1,00	 |	   |         |         | Strong positive
-------------|---------|---------|---------|---------|---------|
Low	     |   1,00  |   1,00  |  1,00   | 	     |         | Strong positive
-------------|---------|---------|---------|---------|---------|
Close	     |   1,00  |   1,00  |  1,00   |   1,00  |         | Strong positive
-------------|---------|---------|---------|---------|---------|
Volume	     |   -0,15 |   -0,15 |  -0,15  |   -0,15 |  1,00   | Weak negative
-------------|---------|---------|---------|---------|---------|

The Correlation of Strong Positive means a strong relationship, so when one variable increases, the other increases. 
The Correlation of Weak Negative means that while one variable decreases, the other increases at the same time.
The strong correlation has a range from -1 to +1. 
