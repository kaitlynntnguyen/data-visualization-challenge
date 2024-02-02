# Data Visualization Challenge

This assignment is broken down into the following tasks:

### Prepare the data
  - I ran the provided package dependency and data imports and merged the `mouse_metadata` and `study_results` DataFrames into a single DataFrame.

  - Displayed the number of unique mice IDs in the data and checked for any mouse ID with duplicate time points. Created a cleaned DataFrame where this data is removed.

### Generate summary statistics.
  - Created a DataFrame of summary statistics that included:
      - A row for each drug regimen with regimen names contained in the index column.
      - A column for: mean, median, variance, standard deviation, and SEM of the tumor volume.

### Create bar charts and pie charts.
  - Created a bar chart with the Pandas `DataFrame.plot()` method and a second bar chart with Matplotlib's `pyplot` methods.

  - Created a pie chart with the Pandas `DataFrame.plot()` method and a second pie chart with Matplotlib's `pyplot` methods.
    
### Calculate quartiles, find outliers, and create a box plot.

1. Created a grouped DataFrame that shows the last (greatest) time point for each mouse, then merged this grouped DataFrame with the original cleaned DataFrame.

2. Created a list that holds the treatment names and a second, empty list to hold the tumor volume data.

  - Loop through each drug in the treatment list, locating the rows in the merged DataFrame that       correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty    list.

3. Determine outliers by using the upper and lower bounds, and then print the results.

4. Generated a box plot ssing Matplotlib that shows the distribution of the final tumor volume for all the mice in each treatment group and highlight any potential outliers in the plot by changing their color and style.

### Create a line plot and a scatter plot.
  - Generated a line plot of tumor volume versus time point for a single mouse that was treated with Capomulin

  - Generated a scatter plot of tumor volume versus mouse weight for the entire Capomulin treatment regimen.

### Calculate correlation and regression.
  - Calculated the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

  - Plot the linear regression model on top of the previous scatter plot.

