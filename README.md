# Python-Data-Analysis-Automated-QuickStart

This is a Juypiter notebook that automates the exploratory data analysis for any data set that you have uploaded to Juypiter. It prompts you to enter the address of the data file within Juypiter, and then creates a new notebook with the data analysis results. It performs various tasks such as importing the necessary libraries, reading the data into a pandas dataframe, running descriptive statistics, creating visualizations, checking for null values, listing unique values, and performing the Augmented Dickey-Fuller (ADF) test for stationarity.

## How to use it

To use this notebook, you need to have Juypiter installed on your computer or access it online. You also need to have the data file that you want to analyze uploaded to Juypiter. The data file should be in CSV format and have a header row with the column names.

To run this notebook, follow these steps:

1. Open this notebook in Juypiter and run the first cell. It will ask you to enter the address of the data file within Juypiter. For example, if your data file is called Rainfall_data.csv and it is in the data subfolder of Juypiter, you can enter /data/Rainfall_data.csv.
2. After you enter the address of the data file, press Enter. The notebook will validate the data file name and print "Data file found." if it is valid, or "Data file not found. Please check the name and try again." if it is not valid.
3. If the data file is valid, the notebook will create a new notebook with the same name as the data file name (excluding the extension) and save it in the same directory as this notebook. For example, if your data file is called Rainfall_data.csv, the new notebook will be called Rainfall_data.ipynb.
4. Open the new notebook in Juypiter and run all the cells. You will see the data analysis results for your data set. You can also modify or add more cells as you wish.

## What it does

This notebook performs various tasks to help you with your exploratory data analysis. Here is a summary of what each cell does:

- Header: This cell creates a markdown cell with a title that indicates which data set you are analyzing.
- Import Libraries: This cell imports the necessary libraries for data analysis, such as pandas, numpy, matplotlib, and seaborn.
- Read CSV: This cell reads the data from the CSV file into a pandas dataframe called df.
- Head: This cell runs df.head() to show the first five rows of the data set.
- Info: This cell runs df.info() to show the summary information of the data set, such as number of rows, columns, data types, and memory usage.
- Describe: This cell runs df.describe() to show the descriptive statistics of the numerical variables in the data set, such as mean, standard deviation, minimum, maximum, quartiles, and count.
- Histograms: This cell runs df.hist() to create histograms for each numerical variable in the data set. Histograms show the distribution and frequency of values in each variable.
- Correlation Heatmap: This cell creates a correlation heatmap using seaborn. A correlation heatmap shows the pairwise correlation between the numerical variables in the data set. Correlation measures how two variables are related to each other. A positive correlation means that they move in the same direction, while a negative correlation means that they move in opposite directions. A correlation close to 1 or -1 means that they are strongly correlated, while a correlation close to 0 means that they are weakly correlated or independent.
- Boxplots: This cell creates a boxplot for each numerical variable using pandas. A boxplot shows the distribution and outliers of each variable. A boxplot consists of a box that represents the interquartile range (IQR), which is the difference between the 25th and 75th percentiles of the data. The line inside the box represents the median (50th percentile) of the data. The whiskers extend from
the box to 1.5 times the IQR or to the minimum or maximum values of
the data, whichever is smaller or larger. The points outside
the whiskers represent outliers or extreme values of
the data.
- Scatterplot Matrix: This cell creates a scatterplot matrix using pandas. A scatterplot matrix shows
the relationship and trend between each pair of numerical variables in
the data set. A scatterplot shows how two variables vary together by
plotting their values as points on a two-dimensional plane. A positive
slope means that they have a positive correlation,
while a negative slope means that they have a negative correlation. A
flat slope means that they have no correlation or a weak correlation.
- Countplots: This cell creates a countplot for each categorical variable using seaborn. A countplot shows the frequency of each category in a variable by plotting the number of occurrences of each category as bars. A categorical variable is a variable that has a finite number of possible values, such as gender, color, or type.
- Null Value Check: This cell runs a check for null values in each column and prints the counts using pandas. Null values are missing or unknown values in the data set that can affect the analysis and modeling. This cell shows how many null values each column has and what percentage of the total values they represent.
- List Unique Values for Non Numerical Columns: This cell lists the unique values for non numerical columns using pandas. Non numerical columns are columns that have data types other than numbers, such as strings, booleans, or dates. This cell shows the different values that each non numerical column has and how many times they appear in the data set.
- ADF Test: This cell performs the Augmented Dickey-Fuller (ADF) test for each numerical variable using statsmodels. The ADF test is a statistical test to check if a time series is stationary or not. Stationarity means that the statistical properties of the data, such as mean, variance, and autocorrelation, do not change over time. Stationary data is easier to model and forecast than non-stationary data, which may have trends, seasonality, or other patterns that affect the analysis. The ADF test calculates a test statistic and compares it with critical values at different significance levels. If the test statistic is less than the critical value, we can reject the null hypothesis and conclude that the data is stationary. If the test statistic is greater than or equal to the critical value, we cannot reject the null hypothesis and conclude that the data is non-stationary.

## Conclusion

This notebook is a useful tool to automate the exploratory data analysis for any data set that you have uploaded to Juypiter. It saves you time and effort by creating a new notebook with the data analysis results for you. You can use this notebook as a starting point for your data analysis and modify or add more cells as you wish. You can also share this notebook with others who are interested in your data analysis.

I hope you find this notebook helpful!
