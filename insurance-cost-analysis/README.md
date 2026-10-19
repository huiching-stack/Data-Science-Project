# Insurance Cost Analysis (Data Analytics & Machine Learning Project)

This project is part of the IBM Data Analyst / Machine Learning professional coursework, focusing on exploratory data analysis and predictive modeling to estimate medical insurance charges.

## 📋 Project Workflow
1. **Data Importing & Preprocessing:** Loaded the medical insurance dataset, handled missing values (`?` entries) by imputing continuous variables with means and categorical variables with the most frequent value, and formatted numerical data types.
2. **Exploratory Data Analysis (EDA):** Visualized relationships between medical charges and attributes like BMI and smoking status using Seaborn (`regplot`, `boxplot`) and analyzed the correlation matrix.
3. **Model Development:** 
   - Built a single-variable Linear Regression model using the `smoker` attribute.
   - Expanded to a multi-variable Linear Regression model incorporating all attributes.
   - Built a training pipeline utilizing `StandardScaler`, `PolynomialFeatures`, and `LinearRegression` to enhance prediction accuracy ($R^2$ score).
4. **Model Refinement:** Split data into training and testing sets, applied Ridge regression with different alpha values, and evaluated polynomial transformations to prevent overfitting.

## 🛠️ Technologies Used
* **Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib
