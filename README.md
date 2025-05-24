# 10K Financial Trend Analysis with Pandas

## Project Overview

This repository contains the solution for Task 1 of the Boston Consulting Group (BCG) Forage Generative AI Virtual Internship (https://www.theforage.com/simulations/bcg/gen-ai-anlo). As a junior data scientist on the GenAI consulting team, my primary objective was to perform foundational data extraction and initial analysis of financial documents (10-K filings) for key companies. This analysis is a crucial first step towards developing an AI-powered chatbot designed to provide insights from financial reports.

The project demonstrates core data science skills in extracting, cleaning, and analysing structured financial data to identify significant trends and indicators.

## Objectives

* **Data Extraction:** Learn and apply techniques to extract specific financial data points from company 10-K documents.
* **Financial Trend Identification:** Conduct a basic financial analysis to identify year-over-year trends and key performance indicators.
* **Data Preparation:** Format and clean raw financial data to ensure it is suitable for further processing and integration into an AI model.

## Data Source

The financial data for this analysis was sourced directly from the 10-K annual reports of three major companies:
* **Microsoft**
* **Tesla**
* **Apple**

Data points for Fiscal Years 2022, 2023, and 2024 were collected for:
* Total Revenue ($M)
* Net Income ($M)
* Total Assets ($M)
* Total Liabilities ($M)
* Cash Flow from Operating Activities ($M)

The raw data is provided in the `financial_data.csv` file within this repository.

## Technologies Used

* **Python**
* **Pandas:** Extensively used for data manipulation, cleaning (e.g., removing commas, type conversion), and advanced analysis (e.g., `groupby`, `pct_change`, aggregation).
* **Jupyter Notebook:** For interactive development, code execution, and presenting findings in a clear, narrative format.

## Analysis Highlights

The `financial_analysis_notebook.ipynb` details the full analysis, but key insights include:

* **Data Preprocessing:** Robust cleaning procedures were implemented to handle financial data format inconsistencies (e.g., commas), ensuring accurate numerical calculations. All relevant financial columns were converted to numeric types (`int64`).
* **Year-over-Year Growth Calculation:** New columns were dynamically created to represent the percentage change for each financial metric across consecutive fiscal years, enabling direct comparison of performance trends.
* **Data Preparation:** Financial data was cleaned (e.g., removing commas) and converted to numeric types (`int64`) for accurate calculations. Year-over-year percentage growth metrics were then dynamically calculated for key financial indicators.
* **Company Performance Profiles:**
    * **Microsoft:** Demonstrated **strong, consistent growth** across most metrics. Achieved average revenue growth of ~6.17%, Net Income growth of ~2.62%, and Operating Cash Flow growth of ~7.69%, indicating stable operations.
    * **Tesla:** Characterised by **rapid expansion** with high average asset (~14.66%) and liability (~10.18%) growth, alongside solid average revenue growth (~6.58%). However, Net Income was highly volatile, averaging a decline of ~-11.09%, reflecting profitability challenges.
    * **Apple:** A **mature market leader**, showing largely stable revenue but slight average declines in Net Income (~-3.09%) and Operating Cash Flow (~-1.26%). Its immense scale underpins its stability despite modest percentage changes.

* **Comparative Insights:** The analysis highlights distinct growth stages: Microsoft's balanced and stable growth, Tesla's aggressive but volatile expansion, and Apple's mature, large-scale stability. All generate strong cash flow from operations.
## How to View/Run the Project

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/belle-kochapon/10K-Financial-Trend-Analysis-Pandas.git](https://github.com/belle-kochapon/10K-Financial-Trend-Analysis-Pandas.git)
    ```
2.  **Navigate to the Project Directory:**
    ```bash
    cd 10K-Financial-Trend-Analysis-Pandas
    ```
3.  **Install Dependencies:**
    ```bash
    pip install pandas jupyter
    ```
4.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
5.  **Open the Notebook:** In your browser, open `financial_analysis_notebook.ipynb`.
6.  **Run Cells:** Execute the cells sequentially to see the data loading, cleaning, analysis, and conclusions.

## Files in this Repository

* `financial_analysis_notebook.ipynb`: The main Jupyter Notebook containing all the Python code for data extraction, cleaning, analysis, and findings.
* `financial_data.csv`: The dataset containing the extracted financial metrics.
* `README.md`: This file, providing an overview of the project.

---
