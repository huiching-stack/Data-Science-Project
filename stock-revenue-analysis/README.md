# 📈 Stock and Revenue Data Extraction & Dashboard

## 📌 Project Overview
This project focuses on extracting historical stock price and quarterly revenue data for major companies (such as GameStop and Tesla) using web scraping techniques, cleaning the data with Pandas, and preparing it for financial analysis and dashboard visualization.

---

## 🛠️ Key Steps & Workflow
1. **Web Scraping (`requests` & `BeautifulSoup`):** Downloaded HTML web pages containing historical financial metrics and parsed DOM elements.
2. **Data Parsing & Extraction:** Extracted target HTML tables (`<table>`, `<tr>`, `<td>`) to isolate revenue and stock pricing trends.
3. **Data Cleaning (`pandas`):** 
   * Handled missing values and multi-level headers.
   * Stripped string characters (such as commas and dollar signs) to convert text columns into numeric formats.
4. **Validation:** Structured dataframes ready for visualization and reporting.

---

## 🧰 Libraries Used
* `python`
* `pandas`
* `requests`
* `beautifulsoup4`

---

## 📂 How to Run
1. Clone the repository or download the `.ipynb` file.
2. Open the notebook in Jupyter Notebook or JupyterLab:
   ```bash
   jupyter notebook "Revenue Data and Building a Dashboard.ipynb"

## 🙏 Acknowledgments
- IBM Data Science Professional Certificate — Developed as part of the Python Project for Data Science course curriculum.
