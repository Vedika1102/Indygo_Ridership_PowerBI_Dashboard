# Indygo Ridership PowerBI Dashboard

This project was developed for the Information Visualization course at Indiana University in collaboration with IndyGo.

## Objective

The primary objective of this project was to design and implement a comprehensive **Ridership Dashboard** for **IndyGo** as a foundational step toward a larger **open data platform initiative**. 

Public transit agencies, including IndyGo, face growing pressure to become more transparent, data-informed, and responsive to community needs. However, much of their operational data—though collected—is underutilized or inaccessible to stakeholders and the public.

This dashboard was created to bridge that gap by:

- **Centralizing and visualizing stop-level ridership data** across multiple dimensions (time, route, geography, service type) in a clear, interactive format.
- **Equipping IndyGo planners, analysts, and city officials** with timely insights to improve route planning, frequency adjustments, and resource allocation.
- **Enhancing community engagement and public trust** by making ridership patterns accessible and easy to understand for the general public and local organizations.

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

## Power BI Logic
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


