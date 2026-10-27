# Automobile Sales Statistics & Interactive Dashboard

An end-to-end data analysis and interactive web application built to explore historical automobile sales trends, economic indicators, and the impact of economic recessions using Python, Pandas, Plotly, and Dash.

---

## 🚀 Project Overview

This project consists of two main components:
1. **Exploratory Data Analysis (EDA) & Visualization**: Jupyter notebook analyzing historical automobile sales data using Python data visualization libraries (`Matplotlib`, `Seaborn`, and `Folium`).
2. **Interactive Dashboard**: A web-based analytical dashboard built with **Dash** and **Plotly** that allows users to dynamically filter and view statistical reports for yearly performance and recession periods.

---

## 📊 Key Features & Reports

The interactive Dash application offers two report types:
* **Recession Period Statistics**: Displays average sales fluctuations, vehicle type performance breakdowns, advertising expenditure shares during economic downturns, and the effect of unemployment rates on sales.
* **Yearly Statistics**: Displays yearly sales trends, monthly totals, vehicle type distributions, and advertising expenditure share for any selected year between 1980 and 2023.

---

## 📂 Repository Structure

```text
├── app.py                 # Main Dash web application script
├── notebooks/
│   └── data_analysis.ipynb  # Jupyter notebook containing exploratory plots and analysis
├── requirements.txt       # Project dependencies
└── README.md              # Project documentation

```

---

## ⚙️ Installation & Running the Project

# 1. Clone the repository and enter the directory
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
cd YOUR_REPOSITORY_NAME

# 2. Install the required dependencies
pip install -r requirements.txt

# (Alternative: if you don't have a requirements.txt, install manually)
pip install dash pandas plotly requests matplotlib seaborn folium

# 3. Run the Dash Application
python app.py

---

## 📈 Data Source
The dataset used in this project represents historical automobile sales, pricing, consumer confidence indices, GDP figures, and unemployment metrics sourced via Skills Network Cloud Object Storage.

## 📝 License
This project is open-source and available under the MIT License.
