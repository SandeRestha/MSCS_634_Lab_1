# MSCS 634 – Lab 1: Data Visualization, Preprocessing, and Statistical Analysis

**Name:** Sandesh Shrestha 
**Course:** MSCS 634  
**Assignment:** Lab 1  
**Dataset:** Weather Data (January 1–15, 2025)

---

## Purpose of the Lab
The purpose of this lab was to apply foundational **data visualization**, **data preprocessing**, and **statistical analysis** techniques using Python and Jupyter Notebook.  
By exploring a real-world style dataset (daily weather data), this project demonstrates how to clean, visualize, and summarize data for meaningful insights.

Key objectives included:
- Collecting and loading a dataset into a Pandas DataFrame  
- Creating visualizations to explore patterns and relationships  
- Handling missing values, detecting outliers, and performing data reduction  
- Scaling and discretizing data for further statistical or machine learning use  
- Computing central tendency, dispersion, and correlation metrics  

---

## Key Insights from Analysis

### Data Visualization Insights
- **Scatter Plot:** Showed a mild negative relationship between temperature and humidity — as max temperature increased, humidity tended to decrease slightly.  
- **Line Plot:** Demonstrated day-to-day temperature variation, with mild upward and downward trends across the two-week sample.  
- **Bar Chart:** Highlighted visible peaks around days 10–11, making day-to-day comparison intuitive.  
- **Histogram:** Revealed most temperatures clustered between the mid-40s to low-50s °F, confirming a normal, narrow distribution.  
- **Box Plot:** Showed a compact interquartile range and no extreme outliers.  
- **Pie Chart:** Indicated that slightly more than half the days experienced precipitation during this period.

### Statistical Insights
- **Central Tendency:** Average daily high temperature was around the mid-40s°F, humidity centered in the low-70s%, and wind speed averaged around 6 mph.  
- **Dispersion:** The temperature range spanned roughly 10–11°F, and precipitation values were small but frequent.  
- **Correlation:** Max and Min temperatures were strongly positively correlated, while precipitation and humidity showed weaker relationships.

---

## Challenges and Decisions Made
- **Synthetic Dataset Creation:** Since external downloads were restricted, a 15-day weather dataset was manually created to simulate realistic data.  
- **Missing Values:** Introduced NaNs intentionally to demonstrate imputation; numeric columns were filled using **mean substitution**.  
- **Outlier Handling:** Used the **IQR method** to identify outliers; none were extreme enough to distort analysis, but the step was shown for completeness.  
- **Data Reduction:** Demonstrated both random sampling (70% of rows) and dimension elimination (dropping `Wind_Speed_mph`).  
- **Scaling:** Applied both **Min–Max** and **Z-score** normalization to illustrate rescaling effects.  
- **Discretization:** Grouped `Temp_Max_F` into **Low**, **Moderate**, and **High** categories for categorical interpretation.

---

## Summary
This lab reinforced how each preprocessing and analysis step builds a foundation for deeper machine learning and data analytics tasks.  
The resulting dataset is clean, well-structured, and statistically characterized — ready for modeling, forecasting, or correlation analysis.
