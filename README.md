# Indygo Ridership PowerBI Dashboard

This project was developed for the Information Visualization course at Indiana University in collaboration with IndyGo.

## Objective

Build a dynamic Power BI dashboard that visualizes ridership trends using stop-level data from IndyGo, forming the backbone of a scalable open data platform.

## Dashboard Highlights
- **Total Ridership** by day, week, and month
- **Stop-wise and Route-wise** ridership comparison
- **Time-based trends** (week number, day of week, monthly patterns)
- Interactive map visualizations with drill-down filters

## Dataset Overview
- **Source**: GPS + Automatic Passenger Counters (APCs)
- **Tables**: FactSegmentAdherence, DimStop, DimRoute, DimDate, DimTrip, DimVehicle, DimBlock
- **Timeframe**: 2023–2024
- **Format**: CSVs + Data Dictionary

## 🧠 Power BI Logic
- DAX Measures: `Total Ridership`, `Ridership Last Week`, `Ridership by Day`
- Calculated Columns: `Route Display Name`, `Week Number`
- Relationships: Star schema with fact/dimension model

## Tools Used
- Power BI
- DAX
- Data Modeling
- Map Visuals
- Calendar-based filtering

##  Project Sponsor
- IndyGo


