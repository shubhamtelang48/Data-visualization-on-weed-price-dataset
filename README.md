# Data-visualization-on-weed-price-dataset

- In this weed price dataset ,we use DateTime library to seperates the month and year from given date column and create the new columns for month and year.
- We use groupby function on year and month column for EDA purpose
- Then we use line and histogram graph for data visualization
- After that also use Joinplot and Pairplot library
- We use Dataprep library for EDA
- From Spicy library we calculate the Zscore (z =np.abs(stats.zscore(df['HighQ'])))
- IQR(Inter Quartile Range) approach to finding the outlier is the most commonly used and most trusted approach used in research field.
- IQR = Quartile3 - Quartile1
- Calculate Q1, Q3 and IQR
 Q1 = dfcolumn.quantile(0.25)
 Q3 = dfcolumn.quantile(0.75)
 IQR = Q3-Q1                 #Interquartile range
#In general, constant should be 1.
 lower  = Q1-1*IQR
 higher = Q3+1*IQR
