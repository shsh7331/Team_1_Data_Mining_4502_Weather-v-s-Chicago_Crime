
# Chicago Crime and Max Temp Data Mining

## Team Members
- Patrick Ridley
- Shrey Shah

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


## Project Description
This project investigates the relationship between Chicago crime rates and daily maximum temperatures over a 15-year span (2010–2025). By integrating crime incident data with NOAA weather records, we uncover seasonal patterns and correlations that help inform public safety strategies, emergency preparedness, and urban policy-making.

## Research Question & Findings
**Questions Sought:**
- Does daily maximum temperature influence crime rates in Chicago?
- Which types of violent crimes are most sensitive to changes in temperature?
- How do crime patterns vary seasonally with respect to temperature changes?

**Summary of Answers:**
- Crime rates tend to rise during moderate warm temperatures, with clear peaks during spring and early summer months.
- Assault and battery incidents show a strong positive correlation with daily maximum temperatures.
- Homicides and sex-related crimes demonstrate weak correlations with temperature, suggesting they are influenced by other factors.

## Application of This Knowledge
- **Law Enforcement:** Allocate resources more effectively during high-risk temperature periods.
- **Urban Planning:** Design preventive community safety initiatives based on seasonal crime trends.
- **Emergency Services:** Enhance preparedness for predictable crime surges during moderate weather conditions.
- **Public Awareness:** Promote proactive community engagement during specific seasonal windows.

## Demonstration Video
[Watch our video demonstration here](https://example.com/demo-video)  

## Final Project Paper
[Read our final project paper here](/01_ChicagoCrime_Part4.pdf)  

## Tools & Technologies
- MySQL
- Python (Pandas, Matplotlib, Seaborn)
- SQLAlchemy (recommended for future database operations)
- Microsoft PowerPoint

## Notebook with Code and Descriptions
[Read our final project paper here](/chi_crime_analysis_rev4.ipynb)  

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

© 2025 CSPB 4502 Team 1 | Chicago Crime and Max Temp Data Mining
