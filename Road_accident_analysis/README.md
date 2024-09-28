
# Road Accident Data Analysis

## Dataset Overview

This dataset contains detailed records of road accidents, including various features that provide information about the accident circumstances, location, vehicles involved, and casualties. Each row in the dataset represents a single accident, and the columns provide specific attributes related to that accident.
# Dashboard
![Accident-Dashboard](https://github.com/user-attachments/assets/078e9f16-228a-4daa-a8da-232ae9e346f5)

# Pivot Table used for visualization:
![Chart_data](https://github.com/user-attachments/assets/b959723f-cae9-4aa9-9d8f-b57d890a799f)

## KPIs (Key Performance Indicators)

### Primary KPIs

- **Fatal Casualties**: Accidents resulting in at least one fatality.
- **Serious Casualties**: Accidents resulting in serious injuries.
- **Slight Casualties**: Accidents resulting in minor injuries.

These KPIs are derived from the `Accident_Severity` column and the `Number_of_Casualties` column.

### Secondary KPIs

- **Casualties by Car**: Focus on casualties where a car was involved, as indicated in the `Vehicle_Type` column.
- **Casualties by Other Vehicle Types**: Breakdown of casualties involving other types of vehicles (motorcycles, trucks, buses, etc.).

## Visualization Charts

### 1. Casualties Yearly Line Chart
- **Purpose**: Visualize the trend in the number of casualties over time (yearly).
- **Details**: Plot a line chart with the `Year` on the x-axis and the `Number_of_Casualties` on the y-axis. Different lines can represent fatal, serious, and slight casualties.

### 2. Casualties by Road Type
- **Purpose**: Show the distribution of casualties across different road types.
- **Details**: Create a bar chart with `Road_Type` on the x-axis and the total number of casualties on the y-axis. The bars can be color-coded by accident severity (Fatal, Serious, Slight).

### 3. Casualties by Light Conditions
- **Purpose**: Analyze the effect of lighting conditions on accident casualties.
- **Details**: Use a bar or pie chart to represent the number of casualties under different lighting conditions (e.g., daylight, darkness). Break down by severity for more detailed analysis.

### 4. Casualties by Road Surface Conditions
- **Purpose**: Understand how road surface conditions affect the severity of accidents.
- **Details**: Create a bar chart to show the number of casualties for each road surface condition (e.g., dry, wet, icy). Color-code the bars by accident severity.

### 5. Casualties by Location (Geospatial Analysis)
- **Purpose**: Identify geographical patterns in accidents and casualty distribution.
- **Details**: Create a heatmap or scatter plot using latitude and longitude to visualize where accidents with high casualties are concentrated. This can help highlight dangerous locations or regions.

### 6. Casualties by Vehicle Type
- **Purpose**: Compare casualty counts across different types of vehicles involved in accidents.
- **Details**: A bar chart showing the number of casualties for each vehicle type (e.g., cars, motorcycles, trucks). The x-axis represents the `Vehicle_Type` and the y-axis the `Number_of_Casualties`. Additionally, color-code by accident severity.

## Analysis Workflow

### Step 1: Data Loading
- Load the dataset into a Pandas DataFrame.
- Ensure the data types of each column are correct, especially for date, time, and numerical fields (e.g., `Accident_Severity`, `Number_of_Casualties`, `Latitude`, `Longitude`).

### Step 2: Data Cleaning
- Handle missing data in critical columns like `Junction_Control`, `Carriageway_Hazards`, and `Weather_Conditions`.
- Correct any inconsistencies, such as invalid or missing `Accident_Severity` or `Number_of_Casualties`.

### Step 3: KPI Analysis

#### Primary KPI Analysis
- **Fatal, Serious, and Slight Casualties**: Break down the number of casualties by severity and analyze factors contributing to the severity, such as weather, road type, and light conditions.

#### Secondary KPI Analysis
- **Casualties by Car**: Filter data where `Vehicle_Type = Car` and analyze the number and severity of casualties.
- **Casualties by Other Vehicle Types**: Analyze casualty counts for motorcycles, trucks, buses, and other vehicle types, and compare them to car-related casualties.

### Step 4: Visualization

1. **Yearly Line Chart**:
   - Plot `Year` against the total number of casualties.
   - Different lines for fatal, serious, and slight casualties.

2. **Casualties by Road Type**:
   - Plot a bar chart of `Road_Type` vs. `Number_of_Casualties`.
   - Color the bars based on accident severity.

3. **Casualties by Light Conditions**:
   - Create a bar or pie chart of `Light_Conditions` vs. `Number_of_Casualties`.
   - Break down the chart into categories based on accident severity.

4. **Casualties by Road Surface Conditions**:
   - Show how road conditions influence the number of casualties using a bar chart with road conditions on the x-axis and casualties on the y-axis.

5. **Casualties by Location**:
   - Use latitude and longitude for plotting a scatter plot or heatmap to identify high-risk areas.

6. **Casualties by Vehicle Type**:
   - Plot a bar chart to compare the number of casualties across different vehicle types.

### Step 5: Statistical Analysis

- **Correlation Analysis**: Investigate correlations between variables like road type, light conditions, vehicle type, and accident severity.
- **Geospatial Analysis**: Use geographical data to analyze location-based patterns of accidents and casualties.
- The analysis of road accident data will provide several key insights that can inform policy-making, safety measures, and targeted interventions. Here are some of the primary insights you can expect:


### Overall Strategic Insights:
   - **Policy Recommendations**: Based on insights about accident hotspots, time of day, or contributing factors like lighting and weather, policymakers can make more data-driven decisions to allocate resources effectively and reduce the overall number of casualties.
   - **Public Awareness Campaigns**: Insights into high-risk behaviors (e.g., speeding, nighttime driving, or driving in adverse weather) can inform public campaigns aimed at reducing risky behaviors.
   - **Targeted Safety Measures**: The analysis can help local authorities target infrastructure improvements such as better lighting, road surfacing, or enhanced junction controls in areas identified as accident hotspots.

- In conclusion, this analysis will provide actionable insights to improve road safety, reduce casualties, and help allocate resources to high-risk areas for more effective traffic management and accident prevention efforts.
---
