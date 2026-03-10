# jumia-kitchen-analysis
Web scraping and market analysis of Jumia Nigeria Home &amp; Kitchen products using Python and Power BI


# 🏠 Jumia Nigeria — Home & Kitchen Market Intelligence

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup4-Scraping-green)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Cleaning-150458?logo=pandas)
![PowerBI](https://img.shields.io/badge/PowerBI-Dashboard-F2C811?logo=powerbi)

## 📌 Project Overview
This project performs a full end-to-end data analysis of **Home & Kitchen Appliances** 
listed on **Jumia Nigeria** (jumia.com.ng) — one of Africa's largest e-commerce platforms.

The goal is to answer key business questions about the Nigerian home appliance market:
- Which brands dominate the market?
- What does the price distribution look like?
- Which products offer the best value for money?
- Which categories have the biggest discounts?

---

## 🎯 Business Questions Answered
1. 📦 How many Home & Kitchen products are listed on Jumia Nigeria?
2. 🏭 Which brands have the most product listings?
3. 💰 What is the price distribution across all products?
4. 🏷️ Which products have the highest discounts?
5. ⭐ What are the best value deals available?
6. 💸 Which brands are the most expensive on average?

---

## 🛠️ Tools & Technologies
| Tool | Purpose |
|------|---------|
| `Python 3.11` | Core programming language |
| `BeautifulSoup4` | Web scraping |
| `Requests` | HTTP requests |
| `Pandas` | Data cleaning & analysis |
| `Matplotlib & Seaborn` | Data visualization |
| `Power BI` | Interactive dashboard |
| `Jupyter Notebook` | Development environment |

---

## 📁 Project Structure
```
jumia-kitchen-analysis/
│
├── data/
│   ├── raw/                          ← Raw scraped data
│   │   └── jumia_kitchen_raw.csv
│   └── cleaned/                      ← Cleaned & processed data
│       └── jumia_kitchen_cleaned.csv
│
├── notebooks/
│   ├── 01_scraping.ipynb             ← Web scraping script
│   ├── 02_cleaning.ipynb             ← Data cleaning script
│   └── 03_analysis.ipynb             ← EDA & analysis script
│
├── visuals/                          ← Saved charts & graphs
├── dashboard/                        ← Power BI dashboard file
└── README.md
```

---

## 🔄 Project Workflow

### Phase 1 — Web Scraping
- Scraped **210+ products** from Jumia Nigeria's Home & Kitchen section
- Extracted: product name, price, old price, discount %, and product URL
- Used `requests` and `BeautifulSoup4` to parse HTML
- Handled missing data and pagination across 5 pages

### Phase 2 — Data Cleaning
- Removed duplicate listings
- Cleaned price columns (removed ₦ symbol and commas)
- Extracted brand names from product titles
- Created new calculated columns:
  - `discount_amount` — money saved
  - `discount_pct_calc` — calculated discount %
  - `price_range` — price buckets for distribution analysis
  - `discount_range` — discount buckets for distribution analysis

### Phase 3 — Exploratory Data Analysis
- Analysed price distribution across all products
- Identified top brands by number of listings
- Compared average prices across brands
- Found products with the highest discounts
- Identified best value products

### Phase 4 — Dashboard
- Built an interactive **Power BI dashboard** with 2 pages:
  - **Page 1:** Market Overview (KPI cards, top brands, top discounts, avg price by brand)
  - **Page 2:** Price & Value Analysis (price distribution, market share treemap, best deals table)

---

## 📊 Key Findings
- 🏆 **Nine** is the most listed brand on Jumia Nigeria Home & Kitchen
- 💰 Average product price is **₦44,107** 
- 🔥 Highest discount found is **43%** off
- 📉 Average discount across all products is **26%**
- 💸 **Firman** is the most expensive brand on average
- 🛒 Most products fall in the **₦10,000 - ₦50,000** price range

---

## 💡 How to Run This Project

### 1. Clone the repository
```bash
git clone https://github.com/Temmygabriel/jumia-kitchen-analysis.git
cd jumia-kitchen-analysis
```

### 2. Install dependencies
```bash
pip install requests beautifulsoup4 pandas matplotlib seaborn openpyxl lxml
```

### 3. Run the notebooks in order
```
01_scraping.ipynb   → Scrape fresh data from Jumia
02_cleaning.ipynb   → Clean and process the data
03_analysis.ipynb   → Run the analysis and generate charts
```

### 4. Open the dashboard
- Open `dashboard/jumia_kitchen_dashboard.pbix` in Power BI Desktop

---

## 📬 Connect With Me
- 🐙 GitHub: [github.com/Temmygabriel](https://github.com/Temmygabriel)

---

*This project was built as part of my Data Analyst portfolio to demonstrate 
real-world skills in web scraping, data cleaning, analysis and visualization.*
