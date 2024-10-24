# Electric Vehicle Data Analysis in SQL

## Overview
This project involves analyzing a large dataset of electric vehicles registered in a specific region using SQL. The dataset contains **186,879 records**, each representing a unique electric vehicle. The goal of this analysis is to explore the adoption trends, geographic distribution, and key characteristics of different electric vehicle models. The project includes various SQL queries for data retrieval, manipulation, and summarization.

## Dataset Information
- **Table Name:** `electric_vehicles`
- **Total Number of Rows:** 186,879
- **Dataset Description:** Each row in the dataset corresponds to a registered electric vehicle and includes attributes such as location, vehicle specifications, and utility details.

### Columns Description
- **VIN:** Vehicle Identification Number, a unique identifier (first 10 characters used here).
- **County, City, State, Postal Code:** Geographic location details for registration.
- **Model Year:** Year the vehicle model was manufactured.
- **Make & Model:** Manufacturer and model details.
- **Electric Vehicle Type:** Type of electric vehicle (e.g., BEV, PHEV).
- **CAFV Eligibility:** Eligibility for clean alternative fuel vehicle incentives.
- **Electric Range:** Maximum distance the vehicle can travel on a single charge.
- **Base MSRP:** Manufacturer's Suggested Retail Price for the base model.
- **Legislative District:** District for vehicle registration.
- **Electric Utility:** Utility company providing electric service.

## SQL Queries Overview
- Retrieve basic details like VIN, Make, and Model.
- Filter data by specific conditions like Model Year and Make.
- Perform aggregations such as counting total vehicles, finding averages, and ranking vehicles.
- Use advanced functions like window functions, subqueries, and stored procedures for deeper analysis.
- Create views for categorizing high-end vehicles.
- Categorize electric vehicles based on their range (Short, Medium, Long).

### Key SQL Queries
- **List all electric vehicles with VIN, Make, and Model:**
  ```sql
  SELECT vin, Make, Model FROM electric_vehicles;

