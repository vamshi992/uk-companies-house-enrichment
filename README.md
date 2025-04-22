# 🏢 UK Companies Data Profiling and Enrichment with Companies House API

## 📌 Objective
The objective of this project is to develop a data engineering ETL process that profiles, cleans, deduplicates, and enriches sample company data using the Companies House REST API. This is done to validate and augment UK company contact records with real-time, authoritative data.

## 📂 Dataset
- File: `Csv_file_company.csv`
- Contains sample details of UK-based limited companies.
- Includes fields like company name, address, registration number, etc.

## ⚙️ Key Steps in the Notebook

### 1. Data Loading & Initial Profiling
- Loaded the CSV into a pandas DataFrame.
- Profiled for missing values, column types, and duplicates.

### 2. Data Cleaning
- Standardized company names and postcodes.
- Removed special characters and handled nulls.

### 3. API Integration
- Queried the [Companies House API](https://developer.company-information.service.gov.uk/) using company names.
- Implemented a smart caching system to avoid duplicate requests.

### 4. Data Enrichment
- Extracted fields like company number, status, SIC codes, and address from the API responses.
- Merged enriched data back into the main dataset.

### 5. Visualization
- Visualized:
  - Company status breakdown
  - Top countries of origin
  - Company categories
  - Missing value heatmaps
  - Active vs dissolved companies

## 🧰 Tech Stack
- Python 3
- Pandas
- Matplotlib & Seaborn
- Requests (for API calls)
- Jupyter Notebook

## ▶️ How to Run This Notebook

1. Clone this repository:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```

2. Install the required packages (if not already installed):
    ```bash
    pip install pandas matplotlib seaborn requests
    ```

3. Open the notebook:
    ```bash
    jupyter notebook
    ```

4. Run each cell in order. Make sure to update the `API_KEY` at the top of the notebook.



## 🙋‍♂️ Author
**Vamshi**  
[GitHub](https://github.com/vamshi992)

