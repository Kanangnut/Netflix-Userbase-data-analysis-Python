**Exploratory Data Analysis (EDA) on Netflix Userbase**

This project involves performing exploratory data analysis on a Netflix userbase dataset containing 2,500 rows and 10 columns. The analysis aims to uncover insights about user demographics, subscription patterns, and revenue distribution. The dataset includes information on subscription type, monthly revenue, join date, last payment date, country, age, gender, device, and plan duration.

### Steps and Key Findings:

1. **Data Cleaning and Preprocessing:**
   - Removed the `User ID` column.
   - Checked for missing values and duplicates, finding none.
   - Converted date columns (`Join Date` and `Last Payment Date`) to datetime format.
   - Extracted year and month from the date columns.
   - Calculated the account age (in days) since the join date.
   - Transformed categorical columns (`Subscription Type`, `Country`, `Gender`, `Device`) into dummy variables.
   - Binned the `Age` column into six categories for more granular analysis.

2. **Descriptive Statistics:**
   - The dataset was explored to understand data types, distributions, and memory usage.
   - Plotted the distribution of subscription types, countries, genders, and age groups.
   - Observed that `Basic`, `Premium`, and `Standard` subscriptions had varying user distributions, with `Basic` being the most popular.
   - Created visualizations showing the relationship between age groups, subscription types, and revenue generation.

3. **Visualizations and Insights:**
   - **Subscription Types:** Countplot and pie chart visualizations revealed that the `Basic` subscription is the most common, followed by `Standard` and `Premium`.
   - **Country and Subscription:** A barplot showed the distribution of subscription types across different countries, with the United States having the highest number of subscribers.
   - **Gender Distribution:** A pie chart indicated a near-equal distribution between male and female users.
   - **Age Distribution:** Histograms showed that most users fall within the 28-37 age range.
   - **Device Usage:** Barplots revealed that smartphones are the most used devices, followed by laptops and tablets.
   - **Revenue by Device and Country:** Analysis indicated that laptops generate the highest revenue, and the United States contributes the most to Netflix's monthly revenue.
   - **Subscription Duration:** Plots displayed the correlation between subscription types and plan durations, as well as age groups and plan durations.
   - **Monthly Revenue Trends:** A line plot highlighted seasonal trends in monthly revenue, indicating potential patterns related to user behavior.

### Conclusion:
The EDA on Netflix's userbase provided valuable insights into customer demographics, device preferences, and revenue distribution. The analysis identified key trends, such as the popularity of `Basic` subscriptions, the prevalence of smartphone usage, and the significant contribution of certain countries to Netflix's revenue. These findings can guide strategic decisions in marketing, content creation, and customer retention.
