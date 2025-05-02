# Household Electric Power Consumption Analysis

## 📊 Overview

This project analyzes household electric power consumption over a 2-day period (**February 1–2, 2007**) using data from the [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption). The dataset contains **minute-by-minute measurements** of various electrical quantities for a single household recorded over nearly 4 years.

The goal is to examine how household energy usage varies during the specified period through visualizations created using **R**.

---

## 🗂 Dataset

- **Source**: [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)  
- **File**: `household_power_consumption.txt`  
- **Size**: 20 MB  
- **Description**: Measurements of electric power consumption with a one-minute sampling rate.

### 📌 Variables:

- `Date`: Date in format `dd/mm/yyyy`  
- `Time`: Time in format `hh:mm:ss`  
- `Global_active_power`: Household global minute-averaged active power (in kilowatt)  
- `Global_reactive_power`: Household global minute-averaged reactive power (in kilowatt)  
- `Voltage`: Minute-averaged voltage (in volt)  
- `Global_intensity`: Household global minute-averaged current intensity (in ampere)  
- `Sub_metering_1`: Kitchen energy usage (dishwasher, oven, microwave) in watt-hour  
- `Sub_metering_2`: Laundry room energy usage (washing machine, tumble-drier, refrigerator, light) in watt-hour  
- `Sub_metering_3`: Water heater and air-conditioner energy usage in watt-hour  

---

## 📁 Project Structure

├── household_power_consumption.Rmd # Main R Markdown file for analysis
├── household_power_consumption.md # Rendered Markdown version
├── plot1.R # Script for histogram of Global Active Power
├── plot2.R # Script for time-series line plot
├── plot1.png # Histogram plot
├── plot2.png # Line plot of Global Active Power
├── plot3.png # Line plot comparing Sub-metering 1, 2, and 3
├── plot4.png # Multi-panel plot
└── README.md # Project overview and instructions



---

## 📈 Analysis

The project focuses on a subset of the data for **February 1–2, 2007**, and includes the following visualizations:

- **Plot 1**: Histogram of `Global_active_power`, showing the distribution of power consumption.
- **Plot 2**: Line plot of `Global_active_power` over the 2-day period.
- **Plot 3**: Line plot comparing energy usage from three sub-meters:
  - Sub_metering_1 (Kitchen)
  - Sub_metering_2 (Laundry Room)
  - Sub_metering_3 (Water Heater & AC)
- **Plot 4**: Four-panel plot displaying:
  - Global Active Power  
  - Voltage  
  - Energy Sub-metering  
  - Global Reactive Power  

---

## 🧰 Requirements

- **R** (version 3.6 or higher)

### 📦 R Packages

- `data.table` (for fast and efficient data loading)
- `rmarkdown` (for rendering `.Rmd` files)

> Visualizations use **base R's plotting system**.

---

## 🚀 Installation Instructions

1. Install **R** if not already installed:  
   👉 [https://cran.r-project.org](https://cran.r-project.org)

2. Install required R packages:

```R
install.packages("data.table")
install.packages("rmarkdown")



