# SpaceX Falcon 9 First Stage Landing Prediction
*IBM Data Science Capstone Project*

## 📌 Project Overview
In this capstone project, we predict whether the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website with a cost of $62 million, whereas other providers cost upwards of $165 million each. Much of these savings are achieved because SpaceX successfully reuses the first stage. 

By determining whether the first stage will land, we can estimate launch costs. This predictive capability is valuable for competitors looking to bid against SpaceX or analyze launch economics.

---

## 📊 Project Methodology & Workflow
The project follows a standard data science pipeline:
1. **Data Collection & Wrangling:** Gathering launch data via APIs and web scraping, followed by data cleaning and feature engineering.
2. **Exploratory Data Analysis (EDA):** 
   * Utilizing SQL for data querying and analysis.
   * Using **Pandas** and **Matplotlib/Seaborn** to visualize launch trends (payload mass, launch sites, orbit types, and success rates).
3. **Interactive Visual Analytics:** Building interactive geographic maps with **Folium** to analyze launch site proximity to coastlines, highways, and railways.
4. **Dashboard Development:** Creating an interactive **Plotly Dash** application to filter and explore success metrics dynamically.
5. **Machine Learning Predictive Modeling:** Training classification models (Logistic Regression, SVM, Decision Trees, KNN) to predict first-stage landing outcomes and tuning hyperparameters using GridSearchCV.

---
