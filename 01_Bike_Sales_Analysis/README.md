# 🚲 Cyclistic Bike-Share Analysis

## 📌 Project Overview

This case study is part of the Google Data Analytics Capstone. The goal is to analyze how **casual riders** and **annual members** use Cyclistic bikes differently, and recommend marketing strategies to convert casual riders into annual subscribers.

- 📍 Company: Cyclistic (Chicago-based bike-share program)
- 🎯 Business Objective: Increase the number of **annual memberships**
- 🧩 Key Question: What marketing tactics can convert casual riders into annual members?

---

## 📊 Key Questions

1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

---

## 📁 Data Source

Data was obtained from [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html), provided by Motivate International Inc.

- ✅ 12 monthly CSV files (Jan–Dec 2022)
- ✅ 5.5+ million rows
- 📅 Covers all seasons in 2022
- ⚠️ No personally identifiable information included due to privacy policy

---

## 🛠️ Tools & Technologies

- **Language**: R (RStudio)
- **Libraries**: `tidyverse`, `ggplot2`, `lubridate`, `ggmap`, `scales`
- **Skills**: Data wrangling, data cleaning, data visualisation, geospatial mapping

---

## 🔧 Data Cleaning & Transformation

- Merged all 12 CSV files into one dataset
- Created new fields:
  - `trip_duration` (in minutes)
  - `trip_date`, `trip_start_time`, `trip_weekday`
- Removed invalid data (e.g., trip duration ≤ 0 or < 1 min)
- Deleted unused columns (station IDs and names)

---

## 📈 Key Insights

1. **Trip Frequency**  
   - Members made more trips than casual riders in 2022 (3.3M vs. 2.3M)

2. **Trip Duration**  
   - Casual riders have longer trips (avg. 30 mins) vs. members (avg. 13 mins)

3. **Seasonality**  
   - Casual riders peak in summer (June–July), drop sharply in winter

4. **Weekday vs Weekend**  
   - Members ride more on weekdays (likely commuting); casual riders on weekends

5. **Bike Type**  
   - Docked bikes used only by casual riders — with much longer durations

6. **Geospatial Behavior**  
   - Casual riders favour stations near the lakeshore and tourist areas  
   - Members ride from more distributed city locations

---

## 📊 Visualisations

- 📆 Ride distribution by month and weekday
- 🕒 Hourly ride frequency (faceted by day)
- 🚲 Ride distribution by bike type
- 🗺️ Top 100 most popular starting locations on map (members vs. casuals)

---

## 📢 Recommendations

1. **Target "Member-like" Casual Riders**  
   Identify casuals who ride frequently on weekdays → Offer special membership incentives

2. **Weekend Promotions**  
   Create seasonal/weekend discounts to convert leisure users to annual plans

3. **Expand Station Coverage**  
   Add more docking stations inland (based on usage patterns) to attract more members
