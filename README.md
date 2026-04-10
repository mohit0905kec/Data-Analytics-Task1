# Data Analytics Internship - Task 1: Data Immersion & Wrangling

## Project Overview
This project is part of the **ApexPlanet Software Pvt. Ltd.**. The objective of Task 1 is to become familiar with a dataset and master the foundational steps of data analysis: acquiring, cleaning, and preparing data for further investigation.

## Objective
* Rapidly acquaint with the provided dataset.
* Master data acquisition, cleaning, and preparation.
* Document the dataset structure and identify quality issues.

## Data Dictionary
The following table documents each variable in the `retail_store_sales.csv` dataset, its type, and its business relevance.

| Variable Name | Data Type | Description | Business Relevance |
| :--- | :--- | :--- | :--- |
| **Transaction ID** | String | Unique identifier for each sale. | Essential for tracking individual orders and preventing fraud. |
| **Customer ID** | String | Links purchases to specific customers. | Used to analyze customer loyalty and buying behavior. |
| **Category** | String | Product group (e.g., Beverages, Food). | Helps identify revenue-driving categories. |
| **Item** | String | Specific product name. | Vital for inventory management and sales tracking. |
| **Price Per Unit** | Float | Cost of a single item. | Crucial for calculating margins and total sales. |
| **Quantity** | Float | Number of items in a transaction. | Used to understand average basket size. |
| **Total Spent** | Float | Final amount paid by the customer. | Primary metric for measuring business revenue. |
| **Payment Method** | String | Method of payment (e.g., Credit Card). | Helps in financial reconciliation and fee analysis. |
| **Location** | String | Store location (Online vs. In-store). | Used to compare performance across channels. |
| **Transaction Date**| String | Date the sale occurred. | Vital for identifying seasonal trends and growth. |
| **Discount Applied**| Boolean | Indicates if a promotion was used. | Useful for evaluating marketing campaign impact. |

## Data Quality Assessment
During the initial profiling of the data, the following critical issues were identified:

* **Missing Values:**
    * **Item:** 1,213 missing values.
    * **Price Per Unit:** 609 missing values.
    * **Quantity / Total Spent:** ~604 missing values.
    * **Discount Applied:** 4,199 missing values (~33% of the dataset).
* **Inconsistent Formatting:**
    * The `Transaction Date` column is stored as a string (Object) and requires conversion to a proper datetime format for analysis.
* **Data Integrity:**
    * The dataset contains **0 duplicate rows**, ensuring each transaction record is unique.

## Steps Performed
1. **Data Access & Familiarization:** Analyzed the dataset structure and created a comprehensive data dictionary.
2. **Data Quality Assessment:** Performed profiling to detect missing data, outliers, and formatting errors.
3. **Data Cleaning (In Progress):** Writing Python/Pandas scripts to handle missing values, standardize date formats, and prepare a final analysis-ready dataset.

## Deliverables
* **Data Dictionary:** Included in this README.
* **Cleaning Script:** Python script (to be uploaded).
* **Cleaned Dataset:** Final analysis-ready CSV (to be uploaded).
* **Walkthrough Video:** 3-5 minute LinkedIn video explaining the process.
