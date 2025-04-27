
# Chicago Crime and Max Temp Data Mining Project

## Overview
This project explores the relationship between daily maximum temperatures and crime rates in Chicago. By integrating historical crime data with weather data, we aim to uncover patterns that can inform public safety strategies and policy decisions.

## Objectives
- Analyze correlations between temperature fluctuations and crime rates.
- Identify seasonal crime trends based on temperature changes.
- Provide actionable insights for law enforcement, urban planners, and policymakers.

## Data Sources
- **Chicago Crime Data (2010–2025):** Over 1 million crime incident records.
- **NOAA Weather Data:** Daily maximum (TMAX) and minimum (TMIN) temperatures.

## Data Processing
- **Crime Data:** 
  - Imported into MySQL database.
  - Filtered to violent offenses (Battery, Assault, Homicide, Sex-related crimes).
  - Standardized dates and transformed arrest data to Boolean format.

- **Weather Data:** 
  - Cleaned using pandas to remove incomplete entries.
  - Exported cleaned data into CSV for integration.

- **Integration:** 
  - Merged crime and weather data based on date.
  - Created an aggregated dataset (`crime_weather_data`) with daily crime counts and weather stats.
  - Indexed for efficient OLAP analysis.

## Analysis Techniques
- **Trend Line Analysis:** 
  - Identified seasonal peaks in crime rates corresponding with warmer temperatures.
- **Smoothed Assault Trends:** 
  - Assault incidents follow an inverted-U relationship with temperature, peaking between 70°F–80°F.
- **Pearson Correlation Analysis:** 
  - Assault and battery crimes positively correlated with higher temperatures.
  - Homicides and sex-related crimes showed weak or minimal correlation.

## Key Findings
- Crime rates rise significantly during moderate warm periods (spring and early summer).
- Moderate temperatures promote more outdoor activities, leading to increased assault rates.
- Public awareness and preventive strategies should be emphasized during predictable seasonal patterns.

## Recommendations
- Strategic resource allocation for law enforcement based on temperature forecasts.
- Community initiatives targeting crime prevention during moderate temperature periods.
- Emergency services preparedness for seasonal crime surges.

## Authors
- Patrick Ridley
- Shrey Shah

## Tools & Technologies
- MySQL
- Python (Pandas, Matplotlib, Seaborn)
- SQLAlchemy (recommended for future database operations)
- Microsoft PowerPoint

## How to Run the Analysis
1. Import crime and weather datasets into a MySQL database.
2. Clean and preprocess data using Python scripts.
3. Perform SQL joins and aggregations.
4. Conduct statistical analyses (correlations, trend analyses) using Python.
5. Visualize findings and prepare reports or presentations.

## Notes
- Ensure all datasets are up-to-date and cleaned before analysis.
- For database connections, it is recommended to use SQLAlchemy for compatibility and maintainability.

---

© 2025 Chicago Crime and Max Temp Data Mining Project - CSPB 4502 Team 1
