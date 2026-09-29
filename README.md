# COVID-19
# COVID-19 Data Analysis - India

An exploratory data analysis (EDA) and visualization project analyzing the spread, recovery rates, and impact of COVID-19 across Indian states and union territories.

---

## 📌 Overview

This project analyzes state-level COVID-19 trends in India using data sourced from Kaggle. It covers data cleaning, key epidemiological metric calculations (Active Cases, Recovery Rate, Death Rate), and visualizations highlighting the hardest-hit regions and trends over time.

---

## 📊 Key Highlights & Features

- **Data Preprocessing & Cleaning:**
  - Standardized date formatting and handled duplicate records.
  - Mapped cumulative statistics (`Cured` → `Recovered`).
  - Derived **Active Cases** using the formula:  
    $$\text{Active} = \text{Confirmed} - (\text{Deaths} + \text{Recovered})$$

- **State-Level Aggregations:**
  - Evaluated peak cumulative totals (`max()`) per State/UT.
  - Calculated **Recovery Rate (%)** and **Death Rate (%)** relative to confirmed cases.

- **Visualizations:**
  - **Top 10 Affected States/UTs:** Bar chart ranking regions with the highest confirmed COVID-19 cases.
  - **Top 10 States by Recovery Rate:** Comparison of recovery performance across states.
  - **Timeline Analysis:** Trend visualization tracking confirmed cases over time.

---

## 🛠️ Tech Stack & Libraries

- **Language:** Python
- **Environment:** Google Colab / Jupyter Notebook
- **Libraries Used:**
  - `pandas` — Data wrangling and transformation
  - `kagglehub` — Dataset downloading and retrieval
  - `matplotlib` & `seaborn` — Statistical visualizations and plotting
  - `os` — File path management

---

## 📂 Dataset

- **Source:** Kaggle (`sudalairajkumar/covid19-in-india`)
- **Primary File:** `covid_19_india.csv`
- **Key Columns:** `Date`, `State/UnionTerritory`, `Cured`, `Deaths`, `Confirmed`

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python installed, or run the project directly in Google Colab. Install the required dependencies:

```bash
pip install pandas matplotlib seaborn kagglehub
