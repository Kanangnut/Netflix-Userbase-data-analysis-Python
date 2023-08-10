# Netflix-Userbase-data-analysis

Here's analysis steps:<br>

<b>1.Loading and Data Overview:</b><br>
Import necessary libraries (pandas, numpy, matplotlib, seaborn) and set up configurations.
Read the dataset from a CSV file ("Netflix_Userbase.csv") using pd.read_csv().
Display the number of rows and columns in the dataset using .shape.
Display a sample of 5 random rows using .sample().

<b>Data Cleaning:</b><br>
Drop the "User ID" column from the dataset using .drop().
Convert columns "Join Date" and "Last Payment Date" to datetime format using pd.to_datetime().
Extract year and month from "Join Date" and "Last Payment Date" using the .dt accessor.
Calculate "Account till" (days since joining) using the current date.

<b>Data Transformation:</b><br>
Rename "Plan Duration" column to "Plan Duration(months)" using .rename() method.<br>
Loop through rows to extract the first character of "Plan Duration(months)" using a for loop.<br>

<b>One-Hot Encoding:</b><br>
Perform one-hot encoding on categorical columns "Subscription Type," "Country," "Gender," and "Device" using pd.get_dummies() and pd.concat().<br>

<b>Age Binning:</b><br>
Create age bins using pd.cut() to categorize users into age groups.<br>

<b>Data Visualization:</b><br>
Utilize various visualization techniques to explore the data distribution, relationships, and insights.<br>
The code uses matplotlib and seaborn for visualizations:<br>
 - Bar plots for subscription counts and subscription types by country.<br>
 - Pie chart for gender distribution.<br>
 - Histogram for age distribution.<br>
 - Count plots for subscription types by age bins, age by device, and subscription types by plan duration.<br>
 - Bar plots for monthly revenue by device, by country, and by subscription type.<br>
 - Line plot for monthly revenue trend over time.<br>
Each visualization provides insights into different aspects of the dataset, helping to understand patterns, relationships, and distributions within the data.
