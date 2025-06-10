# New York House Price Analysis

This project explores the real estate market in New York City by analyzing housing prices using statistical methods, data visualization, and basic machine learning models. The analysis was performed as part of a real estate business strategy to understand pricing patterns, optimize agent distribution, and create predictive models.

## Project Objectives

- Understand the distribution and characteristics of NYC house prices.
- Clean and preprocess housing data by removing outliers.
- Analyze relationships between price and key property features (area, beds, baths).
- Segment the city into data-driven zones using clustering.
- Build a simple linear model to estimate house prices.

---

## Dataset Overview

The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/new-york-housing-market/data) and contains the following numerical variables for each property:

- `Price`: Market value of the property (USD)
- `Beds`: Number of bedrooms
- `Bath`: Number of bathrooms
- `Property sqft`: Total area in square feet
- `Latitude`: Geographic coordinate
- `Longitude`: Geographic coordinate

---

## Exploratory Data Analysis (EDA)

1. **Summary Statistics**: Calculated mean, standard deviation, and quartiles.
2. **Outlier Removal**: Used IQR method to remove extreme values.
3. **Key Findings**:
   - Average price: **$845,329**
   - Average beds: **1.44**
   - Average baths: **1.98**
   - Average area: **1,695 sqft**
   - Price distribution: Skewness = 1.32, Kurtosis = 1.53

4. **Visualizations**:
   - Boxplots (before/after outlier removal)
   - Histogram of house prices
   - Scatter plot: Price vs. Area
   - Correlation heatmap

---

## Spatial Analysis with K-Means Clustering

To improve operational efficiency, agents were grouped by zones using **K-Means Clustering** on latitude and longitude data.

- Best cluster count: **5** (based on silhouette score)
- Resulting clusters closely resemble NYC boroughs.
- Visualization: Scatter plot vs. official borough map.

---

## Price Prediction (Linear Regression)

A linear regression model was used to predict house prices based on property area.
