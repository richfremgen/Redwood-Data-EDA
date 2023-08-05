# Redwood-Data-EDA
EDA and PCA on Redwood Tree Data

## 1. Data collection (20 pts)

* Write a summary of the paper and point out things such as the purpose of the study, where the data was collected and the main conclusion.

## 2. Data Cleaning (40 pts)

This data set is quite raw - it contains some gross outliers, inconsistencies, and lots of missing values. Read the Outlier rejection section in the paper carefully and critically. You don't
have to bindly follow their data cleaning method. The  le sonoma-data-all.csv is a simple concatenation of the two  les sonoma-data-log.csv and sonoma-data-net.csv. However, doing the merge of two data  les requires that they are
consistent. nodeid and epoch together provides a unique identifier for one measure. But some other variables are not consistent.

* Check histograms of each variable in two data  les (Plot only the ones that you think are interesting or relevant). Which variable is not consistent? Convert the data to the same range. NO CODE but explain clearly what you did.
* Remove missing data. Comment on the number of missing measurements and the corresponding date and time period.
* The location data is separate in another  le mote-location-data.txt. Incorporate it in the main table. Hint: here the nodeid serves as a key to add columns for height, direction, distance, and tree. State the number of variables in your new data frame.

## 3. Data Exploration (30 pts)

* Make some pairwise scatterplots of some variables. Pick a reasonable time period. Explain your choice and describe your findings.
*  Are any of the predictors associated with Incident PAR? If so, explain the relationship.
*  Each variable of our data basically have three dimensions: value, height and time. Consider each variable as a time series and look at its temporal trend. Generate such plots (value vs time) with height as color cue for at least four variables (Temperature,
Relative Humidity, Incident PAR and Rejected PAR). You can do it for different time scales (during an hour, during a day or during the entire experiment). However, at
least the plots with days as x-axis are required. Comment on the range, continuity and strange behaviors in these variables.
* After PCA analysis, generate a scree plot of the data. Can this data be approximated by some low-dimensional representation?

## 4. Interest Findings (30 pts)

List three interesting findings about your EDA.

## 5. Graph Critique in the Paper (40 pts)

Provide statistical critique of the provided paper.
