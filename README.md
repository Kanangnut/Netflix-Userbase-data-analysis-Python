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

**For the Netflix Exploratory Data Analysis (EDA) project, the following tools and technical concepts were used:**

### Tools:
1. **Python:** The primary programming language used for data analysis.
2. **Pandas:** A powerful data manipulation and analysis library, used for reading, cleaning, and transforming the data.
3. **NumPy:** A library for numerical operations, used for setting random seeds and performing numerical calculations.
4. **Matplotlib:** A plotting library for creating static, animated, and interactive visualizations in Python.
5. **Seaborn:** A Python data visualization library based on Matplotlib, used for making statistical graphics.
6. **Jupyter Notebook:** An interactive environment for writing and running code, used to conduct the EDA.

### Technical Concepts:
1. **Data Cleaning:**
   - **Handling Missing Data:** Checked for and confirmed that there were no missing values in the dataset.
   - **Handling Duplicates:** Identified and removed any duplicate entries in the dataset.
   - **DateTime Conversion:** Converted string representations of dates into proper datetime objects for easier manipulation and analysis.
   - **Feature Engineering:** Created new features such as `Join Year`, `Join Month`, `Last Payment Year`, and `Account till` to derive more insights.

2. **Data Transformation:**
   - **One-Hot Encoding:** Used `pd.get_dummies()` to create dummy variables for categorical columns such as `Subscription Type`, `Country`, `Gender`, and `Device`.
   - **Binning:** Grouped the `Age` column into bins (e.g., "<18", "18-27", etc.) to simplify the analysis and visualize trends across age groups.

3. **Exploratory Data Analysis:**
   - **Descriptive Statistics:** Used Pandas functions to get an overview of the dataset, including data types, column names, and basic statistics.
   - **Visualizations:**
     - **Count Plots:** Showed the distribution of subscription types, devices, countries, and other categorical variables.
     - **Pie Charts:** Visualized the proportion of different subscription types and gender distribution.
     - **Histograms:** Displayed the distribution of ages within the dataset.
     - **Bar Plots:** Illustrated the monthly revenue generated by each device and country.
     - **Line Plots:** Analyzed trends in monthly revenue over time.

4. **Data Interpretation:**
   - Derived insights based on the visualizations, such as identifying popular subscription types, understanding the distribution of subscribers by age, and recognizing revenue patterns across different countries and devices.

These tools and techniques together helped in performing a comprehensive exploratory data analysis of the Netflix user base dataset.
