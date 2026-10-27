# Analyzing Wildfire Activities in Australia 🇦🇺🔥

An exploratory data analysis (EDA) project investigating historical wildfire activities across different regions in Australia from 2005 onwards.

## 📌 Project Overview
This project utilizes Python data analysis and visualization libraries to examine trends, patterns, and characteristics of wildfires in Australia. By analyzing NASA's satellite and fire activity data, this notebook highlights critical periods of high fire activity and compares fire brightness across various Australian regions.

## 📊 Dataset
The dataset used in this project is **Historical Wildfires**, which records fire activities starting from 2005. 
- **Data Source:** [NASA FIRMS (C6 MCD14DL)](https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/c6-mcd14dl) via IBM Skills Network.
- **Key Variables:**
  * **Region:** The 7 distinct Australian regions (e.g., NSW, NT, QL, SA, TA, VI, WA).
  * **Date:** UTC timestamp for 24-hour intervals.
  * **Estimated_fire_area:** Daily sum of estimated fire area ($km^2$) for vegetation fires with >75% confidence.
  * **Mean_estimated_fire_brightness:** Daily mean estimated fire brightness in Kelvin.
  * **Mean_estimated_fire_radiative_power:** Daily mean radiative power in megawatts.

## 🛠️ Built With & Libraries Used
- **Python** (3.8+)
- **Pandas & NumPy** – For data wrangling, cleaning, and manipulation.
- **Matplotlib & Seaborn** – For statistical plotting and data visualization (line graphs, bar plots).
- **Folium** – For geographical mapping and spatial visualization.

## 🚀 Key Tasks & Insights
1. **Time-Series Analysis of Fire Area:** Tracked the average estimated fire area over time, identifying significant peaks (notably between 2010 and 2013, corresponding to major historical wildfire events in Australia).
2. **Monthly & Yearly Trends:** Grouped data by year and month to narrow down precise high-intensity periods.
3. **Regional Comparisons:** Analyzed the distribution of mean estimated fire brightness across different Australian states/regions using Seaborn bar plots.

---

## 📁 Project Directory Structure

```text
Australia_Wildfires_Project/
│
├── data/
│   └── Historical_Wildfires.csv       # Dataset
│
├── notebooks/
│   └── Wildfire_Analysis_Part1.ipynb   # Data Analysis & Static Plots (Part 1)
│
├── app/
│   └── Dash_wildfire_3.py              # Interactive Dash Web Application (Part 2)
│
├── requirements.txt                    # Required Python packages
└── README.md                           # Project documentation
