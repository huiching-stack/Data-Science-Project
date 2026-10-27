# Analyzing Wildfire Activities in Australia 🇦🇺🔥

An exploratory data analysis (EDA) project investigating historical wildfire activities across different regions in Australia from 2005 onwards.

## 📌 Project Overview
This project utilizes Python data analysis and visualization libraries to examine trends, patterns, and characteristics of wildfires in Australia. By analyzing NASA's satellite and fire activity data, this notebook highlights critical periods of high fire activity and compares fire brightness across various Australian regions.

## 📊 Dataset
The dataset used in this project is **Historical Wildfires**, which records fire activities starting from 2005. 
* **Data Source:** [NASA FIRMS (C6 MCD14DL)](https://earthdata.nasa.gov/earth-observation-data/near-real-time/firms/c6-mcd14dl) via IBM Skills Network[cite: 1].
* **Key Variables:**
  * **Region:** The 7 distinct Australian regions (e.g., NSW, NT, QL, SA, TA, VI, WA)[cite: 1].
  * **Date:** UTC timestamp for 24-hour intervals[cite: 1].
  * **Estimated_fire_area:** Daily sum of estimated fire area ($km^2$) for vegetation fires with >75% confidence[cite: 1].
  * **Mean_estimated_fire_brightness:** Daily mean estimated fire brightness in Kelvin[cite: 1].
  * **Mean_estimated_fire_radiative_power:** Daily mean radiative power in megawatts[cite: 1].

## 🛠️ Built With & Libraries Used
* **Python** (3.8+)
* **Pandas & NumPy** – For data wrangling, cleaning, and manipulation[cite: 1].
* **Matplotlib & Seaborn** – For statistical plotting and data visualization (line graphs, bar plots)[cite: 1].
* **Folium** – For geographical mapping and spatial visualization[cite: 1].

## 🚀 Key Tasks & Insights
1. **Time-Series Analysis of Fire Area:** Tracked the average estimated fire area over time, identifying significant peaks (notably between 2010 and 2013, corresponding to major historical wildfire events in Australia)[cite: 1].
2. **Monthly & Yearly Trends:** Grouped data by year and month to narrow down precise high-intensity periods[cite: 1].
3. **Regional Comparisons:** Analyzed the distribution of mean estimated fire brightness across different Australian states/regions using Seaborn bar plots[cite: 1].
