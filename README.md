# HW5_MatPlotLib_Submission

Checked number of mice with a len on unique function for the ID column.

To find all duplicate IDs I used .Count !=1 which took everything that had more that 1 in the value count for the Mouse ID and created a new series.

Sorted by timepoint to get the last timepoint at the bottom then did a drop_duplicates function (keep="last") to keep the last of the dupes in the df.

For loop for all drug names to go through the data and create mean, median, var, std, and SEM by using a loc function on the new df without dupes. Did a groupby.agg function to get all of those values in one function. 

Found the number of mice per drug by doing a agg(count) by a grouped DF of drug regimen. Plotted bars using pandas and matplotlib to get the same chart.

Found the percentage of sex of mice in the study using a pue chart with pandas and matplot. 

Created a new data set using a loc function on the 4 requested drugs for the comparison. From found the quartiles so I could do a IQR and find the outliers. 

From the new data did a box plot showing each drug, the quartiles, and if there was any outliers. Redid it in seaborn because it looks much cooler.

Found one mice who was on Capomulin and plotted its tumor volume going down over time. 

Plotted a scatter plot for weight vs average tumor volume for all mice in the Capomulin trial.

Found the linear regression model and placed it over the scatter plot.
