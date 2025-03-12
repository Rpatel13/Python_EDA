# Atliq Grands - Exploratory Data Analysis (EDA)

## Project Background

This project focuses on performing Exploratory Data Analysis (EDA) on a fictional hospitality company, "Atliq Grands," which operates a chain of luxury hotels across major cities in India. The dataset provided simulates real-world hotel operations, encompassing various aspects such as bookings and revenue.

**Insight and recommendation are provided in the following key area:**

In today's data-driven hospitality industry, understanding customer behavior, identifying revenue patterns, and optimizing operational efficiency are crucial for success. This EDA project aims to:

* **Occupancy Analysis:** Room occupancy by category. Occupancy trends across cities. Weekday vs. Weekend occupancy rates.
* **Revenue Analysis:** Total revenue realized per city. Month-wise revenue trends. Revenue contribution per booking platform (visualized using a pie chart).
* **Customer Ratings Analysis:** Average ratings per city. Ratings distribution across booking platforms.
* **Develop analytical skills:** Practice and demonstrate proficiency in data cleaning, manipulation, visualization, and statistical analysis using Python and relevant libraries.

## Dataset Information

The dataset comprises six CSV files, each containing specific information:

**1.fact_bookings.csv** - Contains booking details such as property ID, booking date, check-in/check-out dates, number of guests, room category, and booking platform.

**2.dim_date.csv** - Provides date information, including weekdays and weekends.

**3.dim_hotels.csv** - Contains hotel property details, including name, category (Luxury/Business), and city.

**4.dim_rooms.csv** - Describes room categories and classifications.

**5.fact_aggregated_bookings.csv** - Aggregated bookings dataset with details on room occupancy and capacity.

**6.new_data_august.csv** - Additional data for the month of August.

## Key Steps in Analysis

**1. Data Loading and Initial Exploration**
* Read CSV files using Pandas.
* Display dataset structure and check for missing values.
* Explore unique values in categorical columns (room category, booking platform, city, etc.).

**2. Data Cleaning**
* Handled missing values using median imputation.
* Removed negative values for guest count.
* Addressed outliers in revenue data using the 3-sigma rule.

**3. Data Transformation**
* Calculated Occupancy Percentage: (successful_bookings / capacity) * 100
* Merged datasets to include hotel and date attributes.
* Categorized days into weekday and weekend bookings.

## Key Findings

* Weekend occupancy rates are significantly higher than weekday rates.
* Revenue realization varies across cities, with Mumbai generating the highest revenue.
* Online booking platforms contribute to a significant share of revenue.
* Business hotels tend to have lower occupancy rates compared to luxury hotels.

## Future Improvements

* Extend the analysis to seasonal trends.
* Implement predictive modeling for demand forecasting.
* Develop interactive dashboards using Plotly or Dash for better visualization.
