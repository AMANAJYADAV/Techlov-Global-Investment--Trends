# Techlov-Global-Investment--Trends

Teclov is an asset management company aiming to make informed investment decisions by analyzing global funding trends. This project is designed to help Teclov’s CEO identify the most promising **funding types**, **countries**, and **sectors** for investment, aligning with their strategy of investing where most others are investing.

---

## 📌 Project Objective

To analyze real-world investment data and deliver actionable insights that align with Teclov's constraints:
- Invest between **$5 to $15 million** per investment round.
- Invest only in **English-speaking countries** for ease of communication.
- Follow global investment trends to identify optimal **funding types**, **countries**, and **sectors**.

---

## Business Understanding

Teclov's investment strategy mirrors that of many early-stage investors:  
> **“Invest where others are investing.”**

Hence, this project analyzes:
- Which **funding type** typically receives investments in the $5M–$15M range.
- Which **countries** receive the most funding globally.
- Which **sectors** dominate investments in those countries.

---

## Data Overview

The data for this project comes from [Crunchbase](https://www.crunchbase.com/) and includes:

| File           | Description                                                            |
|----------------|------------------------------------------------------------------------|
| `companies.csv`| Basic company information                                               |
| `rounds2.csv`  | Investment round details                                                |
| `mapping.csv`  | Maps company sub-sectors to 8 broad main sectors for simplified analysis|

---

##  Project Workflow

### 🔹 1. Data Cleaning
- Merged `companies.csv` and `rounds2.csv` into a unified `master_frame`.
- Ensured lowercase uniformity and removed mismatched company records.
- Cleaned `category_list` and extracted the primary sector.

### 🔹 2. Funding Type Analysis
- Analyzed four types: `venture`, `seed`, `angel`, and `private_equity`.
- Compared average investment amounts to Teclov’s 5–15M USD criteria.

### 🔹 3. Country Analysis
- Identified top 9 countries by total investment amount for the selected funding type.
- Filtered for English-speaking countries from the top 9.

### 🔹 4. Sector Analysis
- Used the mapping file to group sub-sectors into 8 main sectors.
- Created country-specific frames to analyze investment counts and amounts by sector.

### 🔹 5. Deep Sector Analysis
- Built country-specific dataframes `D1`, `D2`, and `D3` for USA, UK, and India.
- Identified:
  - Top 3 sectors by number of investments
  - Companies receiving highest investments per sector

### 🔹 6. Visualizations
- Plotted:
  1. Funding type distribution and average amounts
  2. Top 9 countries by total investment
  3. Sector-wise investment counts for top 3 countries

---

##  Final Business Insights (from `.ipynb` analysis)

| Metric                                | Result                        |
|--------------------------------------|-------------------------------|
| **Best Funding Type**                | Venture                       |
| **Average Venture Investment**       | $11.74 million                |
| **Top 3 English-Speaking Countries** | USA, UK, India                |
| **Top Sector in USA**                | Others                        |
| **Top Sector in UK**                 | Others                        |
| **Top Sector in India**              | Others                        |
| **Top Company in USA (Others)**      | Virtustream                   |
| **Top Company in UK (Others)**       | Electric Cloud                |
| **Top Company in India (Others)**    | FirstCry                      |

---

## 📊 Technologies Used

- Python (Pandas, NumPy)
- Data Cleaning and Transformation
- Data Aggregation and Mapping
- Visualization (Matplotlib, Seaborn)
- Jupyter Notebook


