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
* **Company Performance Profiles:**
    * **Microsoft:** Demonstrated **strong and consistent growth** across all key financial metrics. Average revenue growth was approximately **6.17%**, with healthy average growth in Net Income (~2.62%) and Operating Cash Flow (~7.69%). This indicates stable market demand and efficient operations.
    * **Tesla:** Characterised by **rapid expansion**, particularly in assets (average ~14.66% growth) and liabilities (~10.18%). While showing strong average revenue growth (~6.58%), its Net Income experienced **significant volatility** with an average decline (~-11.09%), pointing to challenges in consistent profitability during its growth phase.
    * **Apple:** Represents a **mature market leader**, showing largely stable revenue but slight average declines in Net Income and Operating Cash Flow over the period. Its immense scale and strong absolute financial figures underscore its stability, even with more modest or flat percentage growth rates.
* **Comparative Analysis:** The project highlights the varying growth stages and financial health profiles of these tech giants, from Microsoft's steady and balanced growth to Tesla's aggressive expansion, and Apple's mature stability.

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
