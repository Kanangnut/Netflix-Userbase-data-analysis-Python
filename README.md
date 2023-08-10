# Netflix-Userbase-data-analysis

Here's analysis steps:

<b>1.Loading and Data Overview:</b><br>
Import necessary libraries (pandas, numpy, matplotlib, seaborn) and set up configurations.
Read the dataset from a CSV file ("Netflix_Userbase.csv") using pd.read_csv().
Display the number of rows and columns in the dataset using .shape.
Display a sample of 5 random rows using .sample().
Data Cleaning:

Drop the "User ID" column from the dataset using .drop().
Convert columns "Join Date" and "Last Payment Date" to datetime format using pd.to_datetime().
Extract year and month from "Join Date" and "Last Payment Date" using the .dt accessor.
Calculate "Account till" (days since joining) using the current date.
Data Transformation:

Rename "Plan Duration" column to "Plan Duration(months)" using .rename() method.
Loop through rows to extract the first character of "Plan Duration(months)" using a for loop.
One-Hot Encoding:

Perform one-hot encoding on categorical columns "Subscription Type," "Country," "Gender," and "Device" using pd.get_dummies() and pd.concat().
Age Binning:

Create age bins using pd.cut() to categorize users into age groups.
Data Visualization:

Utilize various visualization techniques to explore the data distribution, relationships, and insights.
The code uses matplotlib and seaborn for visualizations:

Bar plots for subscription counts and subscription types by country.
Pie chart for gender distribution.
Histogram for age distribution.
Count plots for subscription types by age bins, age by device, and subscription types by plan duration.
Bar plots for monthly revenue by device, by country, and by subscription type.
Line plot for monthly revenue trend over time.
Each visualization provides insights into different aspects of the dataset, helping to understand patterns, relationships, and distributions within the data.
