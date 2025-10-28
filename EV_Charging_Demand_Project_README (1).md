# Electric Vehicle Charging Demand Forecasting

## Overview
The Electric Vehicle Charging Demand Forecasting project focuses on predicting power demand at EV charging stations based on time, weather, and traffic conditions. This project demonstrates the integration of multiple datasets, the application of forecasting models, and the creation of visualization dashboards for real-world decision-making.

## Objective
To forecast EV charging station demand using statistical and time-series models while identifying influencing factors like temperature, humidity, and traffic flow. The outcome supports optimized charging infrastructure planning and resource management.

## Tools and Technologies
- Python (VS Code)
- Pandas, NumPy
- Prophet (Facebook/Meta Prophet)
- ARIMA (statsmodels)
- Matplotlib, Seaborn
- Openpyxl
- Excel
- Tableau
- python-pptx, reportlab, Pillow (for report and slide generation)

## Dataset
The dataset was created by merging:
- EV usage data (hourly station-level demand)
- Weather data (temperature, humidity, rainfall)
- Traffic index data (congestion percentage)

Derived columns include Hour, Day, and Traffic_Level, categorized as Low, Moderate, or High.  
File used: **EV_Charging_Demand_BaseData_Final.xlsx**

## Methodology
1. **Data Preparation** – Cleaned and merged datasets using Python and Excel.  
2. **Exploratory Data Analysis** – Identified patterns in demand against weather and traffic.  
3. **Forecast Modeling** – Used Prophet for time-series forecasting.  
4. **Visualization** – Built Tableau dashboards to display demand patterns, heatmaps, and KPIs.

## Forecasting
The forecasting model was developed using the Prophet library in Python.  
Separate models were trained for each station to predict hourly demand.  
Accuracy achieved: 91–93% with MAPE between 8–10%.  
Output stored in **EV_Charging_Demand_Forecast_AllStations.xlsx**

## Visualizations
Interactive Tableau dashboard includes:
- Actual vs Forecast Demand Line Chart  
- Hourly Demand Heatmap  
- Traffic Impact Bubble Chart  
- Weather vs Demand Bar Chart  
- KPI Summary Panel for all stations

## Key Insights
- Peak charging hours: 8–10 AM and 6–8 PM  
- Low demand during 12 AM – 5 AM  
- High traffic correlates with higher charging demand  
- Rainy weather reduces overall demand by approximately 15%

## Deliverables
- Forecasting Model (Python - Prophet)  
- Preprocessed Dataset (Excel)  
- Interactive Dashboard (Tableau)  
- Strategic Recommendations for load balancing and optimization  
- Project Report and Presentation

## Conclusion
The project successfully forecasts EV charging demand with high accuracy and provides visual insights into the influence of external parameters like traffic and weather. These insights enable effective planning, load optimization, and infrastructure development for electric vehicle charging networks.