# Uber Ride Hailing Analysis — Summary

This project analyzes ~6,945 Uber ride records to understand demand patterns, cancellations, revenue drivers, and service gaps across time, location, and ride types.

## Data Collection & Cleaning
- Dataset includes timestamps, locations, trip cost, tips, ride type, payment method, driver ID, status, and weather.  
- Converted timestamps and created features: request_hour, dayofweek, wait_time, and trip_duration.  
- Retained cancelled / no-car trips for cancellation analysis; excluded them from duration/revenue metrics.  
- Encoded categorical fields and labeled hours as peak vs off-peak.

## Data Analysis
- **Demand Peaks:** 8–10 AM and 6–8 PM; highest supply shortfall at 6–7 PM.  
- **Day Trends:** Weekday evenings → commute-heavy; weekends → leisure spikes.  
- **Cancellations:** ~25% during peak hours; “No Cars Available” concentrated in major hubs (Majestic, Koramangala).  
- **Revenue Mix:**  
  - UberGo ~33% of trips but ~28% revenue  
  - UberXL ~32% of trips but ~40% revenue  
- Tip amount moderately correlates with trip duration (r≈0.45).

## Visualizations
- Heatmap of requests by hour and pickup area  
- Hourly fulfillment-rate line chart  
- Bar charts for cancellation / no-car rates by ride type & payment method  
- Box plots for wait times and durations  
- Scatter of trip cost vs duration (weather-colored)

## Key Insights
- Rainy/stormy conditions increase cancellations and no-car events by 15–20%.  
- Peak-hour driver shortages create major service gaps.  
- High-value ride types (UberXL) outperform in revenue share.  
- Late-night demand is rising without matching driver availability.

