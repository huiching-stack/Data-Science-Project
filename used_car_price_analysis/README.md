# Used Car Price Analysis & Predictive Modeling (GenAI-Assisted Workflow)

## Project Overview
This project explores a used car pricing dataset (`used_car_price_analysis.csv`) to identify key factors influencing vehicle resale value and build regression models to predict car prices. Developed as part of the **IBM Generative AI for Data Scientists** curriculum, this project demonstrates how prompt engineering can accelerate end-to-end data science workflows—from data cleaning and exploratory data analysis (EDA) to machine learning pipeline optimization.

---

## Repository Structure
* `used_car_price_analysis.ipynb` – Complete Jupyter Notebook containing data preprocessing, visualizations, and regression modeling.
* `requirements.txt` – Required Python libraries to run the notebook locally.

---

## Workflow & Methodology

### 1. Data Preprocessing & Cleaning
* Loaded the dataset using `pandas` and inspected missing values across features.
* Imputed missing numerical values using column means and removed duplicate records to ensure data integrity.

### 2. Exploratory Data Analysis (EDA)
* **Correlation Analysis:** Identified the top 5 numerical features most strongly correlated with `price`:
  1. **Year** (`0.64`)
  2. **Mileage** (`0.53`)
  3. **Engine Size** (`0.41`)
  4. **Tax** (`0.41`)
  5. **MPG** (`0.35`)
* **Categorical Distribution:** Analyzed vehicle counts across `fuelType` categories (Petrol, Diesel, Hybrid, Electric, Other).
* **Visualizations:** Generated Seaborn box plots to examine price distributions and outliers across `transmission` types, and regression plots to visualize the relationship between `mpg` and `price`.

### 3. Predictive Modeling & Evaluation
Trained and evaluated multiple regression models using an 80/20 train-test split (`random_state=42`):

| Model / Pipeline | Features Used | $R^2$ Score | Mean Squared Error (MSE) |
| :--- | :--- | :---: | :---: |
| **Simple Linear Regression** | `mpg` | `0.1504` | `19,049,855` |
| **Multiple Linear Regression** | `year`, `mileage`, `tax`, `mpg`, `engineSize` | `0.6917` | `6,912,745` |
| **Polynomial Regression (Degree 2) + StandardScaler** | `year`, `mileage`, `tax`, `mpg`, `engineSize` | `0.1212` | `19,704,750` |
| **Ridge Regression ($\alpha = 0.1$)** | `year`, `mileage`, `tax`, `mpg`, `engineSize` | `0.6917` | `6,912,726` |
| **Polynomial Ridge Regression (Degree 2, $\alpha = 0.1$)** | `year`, `mileage`, `tax`, `mpg`, `engineSize` | `0.6733` | `7,326,175` |
| **GridSearchCV Ridge Regression (Best $\alpha = 0.01$)** | `year`, `mileage`, `tax`, `mpg`, `engineSize` | `0.3827` | `13,840,985` |

---

## Key Takeaways
* **Feature Impact:** Vehicle age (`year`) and usage (`mileage`) are the strongest predictors of used car price, while fuel efficiency (`mpg`) alone explains only ~15% of price variance.
* **Model Performance:** Standard Multiple Linear Regression and Ridge Regression ($\alpha = 0.1$) achieved the best performance ($R^2 \approx 0.692$), outperforming unscaled higher-degree polynomial transformations which suffered from multicollinearity/ill-conditioning.
* **GenAI Integration:** Leveraging structured prompts significantly reduced boilerplate coding time for data wrangling, visualization formatting, and hyperparameter tuning.
