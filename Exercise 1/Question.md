

Exercise 1

TKO_7093 Statistical Data Analysis
1.

Download the file allbp.data from the Thyroid Disease Data Set available at https://archive.ics.uci.edu/ml/datasets/Thyroid+Disease (see the files in the Data Folder).

Load and preprocess the data so that it is ready for analysis. (Check categorical variables, missing values, variable names and so on.) Use the file allbp.names to your advantage.

    How many observations and how many variables are there in the data?

    Which variables have missing values? How many?

2.

Using the data you prepared above,

    for each variable that has only yes/no values, calculate the number of yes values divided by the number of observations.

    for each of the TSH, T3, TT4, T4U, FTI and TBG variables, calculate the sum of the squared values divided by the number of non-NA values.

    calculate the mean ratio between T3 and TT4.

3.

Load the data available in the file 13-data.csv.

    Find invalid values in the data and replace them either with a correct value (if possible) or with NaN.

    Replace all missing values of the purchases variable with zero.

    Use median imputation to fill in all missing values of the retention_time variable.
    (BONUS) Group the observations by sex and location before calculating the substitute median(s).

4.

The files 14-helsinki.csv and 14-espoo.csv contain daily numbers of cyclists spotted on selected streets in Helsinki and Espoo. Load the files and merge the data into a single data frame.

    For how many days were observations made in total?

    How many observation days were there for each street?

    On how many days were all streets observed simultaneously?

    Which street was the busiest in terms of the total number of cyclists?

    Filter out the dates which have one or more missing values. Does this affect your conclusion about the busiest street? Why or why not?

