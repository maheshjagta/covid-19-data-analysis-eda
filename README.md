# covid-19-data-analysis-eda
Exploratory Data Analysis (EDA) of COVID-19 data using Python: data cleaning, outlier treatment, and univariate, bivariate and multivariate analysis with visual insights.


🦠 COVID-19 Patient Data Analysis
📖 About the Project
This project is an Exploratory Data Analysis (EDA) of COVID-19 data from 10 countries. It uses Python in a Jupyter Notebook to clean the data, handle unusual values, and draw visual insights about cases, deaths, recoveries, vaccination and risk level.

🎯 Goal
The aim is to turn raw, messy COVID-19 records into a clean, understandable dataset. Along the way, the analysis looks at how the numbers are spread, how they compare across countries, and how they relate to each other.

📂 About the Dataset
Size: 1,100 records and 8 columns
Coverage: 10 countries
Columns: Date, Country, Cases, Deaths, Recovered, Active, Vaccine and Risk
Risk: a simple Yes/No indicator
Quality: no duplicate records, but a few missing values
🛠️ Tools Used
🐼 Pandas for loading and cleaning the data
🔢 NumPy for numerical operations
📊 Matplotlib and Seaborn for charts and visualizations
📓 Jupyter Notebook as the working environment
🔄 What Was Done, Step by Step
1. 🔍 Understanding the data
I checked the first and last rows, the number of rows and columns, column names, data types and a statistical summary (average, minimum, maximum and so on).

2. 🧹 Cleaning the data

Missing values were found in three columns, 8 each: Country, Recovered and Vaccine.
Missing numbers were filled with the median, and the missing country was filled with the most common one.
No rows were deleted, and no duplicate records were found.
3. 📦 Handling outliers

Boxplots showed extreme values in the Active cases column.
These were limited to a maximum cap of about 415,000, calculated with the IQR method, so very large values don't distort the analysis.
4. 📊 Single-variable analysis
I studied each column on its own: the spread of Cases, Deaths, Recovered and Active, the number of records per country, and the balance between risk "Yes" and "No".

5. 📈 Two-variable analysis
I compared Cases with Deaths, Cases with Active cases, Active cases across countries, and Active cases by risk category.

6. 🔗 Multi-variable analysis

Cases and Deaths were compared again with Risk shown as colour.
A correlation heatmap showed how strongly Cases, Deaths, Recovered and Active move together.
7. 💾 Saving the result
The cleaned dataset was exported as a new file, ready for future analysis or machine learning.

💡 Key Takeaways
✅ The data was cleaned without losing any records.

📦 Active cases had extreme values that needed controlling.

🌍 The data covers 10 countries, so country-to-country comparison is possible.

⚠️ Risk is a Yes/No feature, which could be used to build a prediction model later.

🔗 The correlation heatmap shows how the main COVID-19 measures are connected.

🔮 Future Scope

📅 Time-based trend analysis using the Date column

🤖 A machine learning model to predict risk

📉 Death rate and recovery rate for each country

💉 The effect of vaccination on deaths and active cases

🗺️ Interactive dashboards, for example with Power BI or Streamlit



🎓 Skills Demonstrated
Data cleaning, missing value handling, outlier detection, data visualization, statistical thinking and storytelling with data.
