
# 🚗 Smart Dynamic Pricing Engine for Urban Parking Lots
**Summer Analytics 2025 – Capstone Project**  
By Ashish Singh

---

## 📌 Project Overview

This project simulates a **real-time dynamic pricing engine** for urban parking lots using historical data. The solution combines economic logic, data science, and live data streaming to create a smart, adaptive pricing system that adjusts based on demand, traffic, location, and competitive factors.

✅ Built using only `pandas`, `numpy`, `bokeh`, and `pathway`.

---

## 📊 Features

- 🔁 **Three Pricing Models**
  - **Model 1 – Linear Pricing**: Increases price linearly with occupancy.
  - **Model 2 – Demand-Based Pricing**: Adds logic for queue length, vehicle type, traffic, and special days.
  - **Model 3 – Competitive Pricing**: Uses geo-location to adjust pricing against nearby parking lots.

- ⚡ **Real-Time Streaming**
  - Powered by **Pathway** to simulate time-ordered streaming of historical data.

- 🎨 **Interactive Dashboard**
  - Built using **Bokeh** for exploring pricing over time across different lots.
  - Features dropdown selection and hover tooltips.

---

## 🏗️ Architecture

graph TD
  A[CSV Dataset] -->|streamed| B(Pathway Engine)
  B --> C{Model 1/2/3 Logic}
  C --> D[Live Price Output]
  D --> E[Bokeh Dashboard]
