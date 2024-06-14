# Road Accident Analysis Project
![](https://github.com/yanny-alt/Road-Accident-Analysis-Using-Power-BI/blob/main/Images/Analysis%20Of%20Road%20Accident%20Trends.jpg)
## Executive Summary

### Background of the Project
In an era where data-driven decisions are crucial, analyzing road accident data can significantly enhance public safety. This article details my Power BI project on road accident analysis, focusing on the UK. By transforming extensive datasets from Kaggle into actionable insights, I aimed to identify patterns and trends that could help mitigate accidents. This case study showcases my proficiency in data visualization and analytics, demonstrating how data can drive strategic decisions to enhance road safety.

### Key Insights Categorized

#### Broad Assessment of Accident Data:
- The dataset includes accidents from 2021 and 2022 in the UK, with detailed records on date, time, location, weather conditions, and vehicle types.
- Significant patterns and trends were identified that can inform safety measures.

#### Key Insights Uncovered:
- **Peak Accident Times**: Identified rush hours and specific days with higher accident rates.
- **High-Risk Locations**: Highlighted intersections and road segments with a high frequency of accidents.
- **Impact of Weather**: Showed a significant correlation between adverse weather conditions and increased accident severity.
- **Total Casualties and Accident Values**: Provided KPIs for current year and year-over-year growth.

### Business Recommendations
- **Local Authorities and Transportation Departments**:
  - Conduct comprehensive safety audits of high-risk zones.
  - Enhance traffic enforcement in high-accident areas.
- **Law Enforcement Agencies**:
  - Strengthen traffic enforcement in identified high-risk zones.
- **Road Safety Organizations**:
  - Launch public awareness campaigns on road safety.
- **Technological Innovators**:
  - Deploy advanced traffic management systems and speed-limiting devices.
- **Data Analysts and Researchers**:
  - Continuously monitor and analyze traffic data to inform policy decisions.

### Dashboard Screenshot
![Dashboard Screenshot](https://app.powerbi.com/view?r=eyJrIjoiMThkM2IzMjAtMTc2YS00ZDE2LTg1ZDktYzVjOTlmOGZmNzE4IiwidCI6IjQ5MWM2ZTNhLTA3MjItNDhmMi1iMDFhLWFhMzliODc0MGYxNiJ9)

## Main Dashboard
The Power BI dashboard we created visually presents the key insights and metrics derived from the dataset. It allows stakeholders to interactively explore the data and gain a better understanding of Road accidents trends around The United Kingdom

![](https://github.com/yanny-alt/Road-Accident-Analysis-Using-Power-BI/blob/main/Images/Road%20Accident%20Tracking%20Dashboard.png)



### Interactive Features
- **Slicers and Filters**: Enabled users to drill down into specific data segments, such as filtering by date, location, or weather condition.
- **Dynamic Visualizations**: Show values changing with different filters, enhancing interactivity.

### Insights by Condition
- **Dry Road Insights**: Analysis of accidents on dry roads.
- **Wet Road Insights**: Analysis of accidents on wet roads.
- **Rainy Weather Insights**: Analysis of accidents during rainy weather.
- **Fine Weather Insights**: Analysis of accidents during fine weather.

## Data Collection and Preparation

### Data Sources
The dataset used for this analysis was obtained from Kaggle. It included detailed records of traffic accidents, covering aspects such as date, time, location, weather conditions, and types of vehicles involved.

### Data Cleaning
To ensure the accuracy and reliability of the analysis, extensive data cleaning was performed:
- **Handling Missing Values**: Filled or removed missing data where necessary.
- **Standardizing Formats**: Ensured consistent date, time, and categorical data formats.
- **Removing Duplicates**: Eliminated duplicate entries to prevent skewed results.

### Data Modeling
Using Power BI’s data modeling features, relationships between different tables were established, including accident details, location data, and weather conditions.

![](https://github.com/yanny-alt/Road-Accident-Analysis-Using-Power-BI/blob/main/Images/Road%20Accident%20Data%20Model.png)

#### Key Steps:
- **Defining Relationships**: Set up primary and foreign keys to link tables.
- **Creating Calculated Columns**: Used DAX (Data Analysis Expressions) for additional calculations like accident severity scores.
- **Calendar Table**: Created a calendar table for time-based analysis.

## Visualizations and Insights

### Primary KPIs
- **Total Casualties and Total Accidents for Current Year and YoY Growth**
- **Casualties by Accident Severity**
- **Casualties by Vehicle Type**

### Trend Analysis
- **Monthly Trend**: Comparison of casualties for current year and previous year.
- **Casualties by Road Type**: Analysis of casualties based on road type.
- **Casualties by Area/Location & Day/Night**: Insights on casualties based on location and time of day.


## DAX Formulas Used in Measures

```DAX
PY Accidents = CALCULATE(COUNT(Data[Accident_Index]), SAMEPERIODLASTYEAR('Calendar'[Date]))
PY Casualties = CALCULATE(SUM(Data[Number_of_Casualties]), SAMEPERIODLASTYEAR('Calendar'[Date]))
YoY Accidents = ([CY Accidents Count] - [PY Accidents]) / [PY Accidents]
YoY Casualties = ([CY Casualties] - [PY Casualties]) / [PY Casualties]

## Conclusion

The Road Accident Analysis project in Power BI has been a rewarding endeavor, enhancing my skills in data visualization, analysis, and storytelling. The insights derived from this project can play a crucial role in improving road safety by informing targeted interventions and policies.

Thank you for reading! Your feedback is appreciated. If you are interested in learning more about my work or discussing potential opportunities, please feel free to connect with me on ![LinkedIn](https://www.linkedin.com/in/favourokechukwu/).


