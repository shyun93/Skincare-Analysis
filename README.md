# Skincare-Analysis
EDA project comparing Western vs Korea skincare products


# 🧴 Korean vs Western Skincare EDA
**Author:** Sarah Hyun  
**Last Updated:** August 2025  
**Tools:** Python, Jupyter Notebook, Pandas, Seaborn, Matplotlib, Selenium

---

## 🧠 Overview

This project explores ingredient trends, pricing, and user ratings across Korean and Western skincare products. Using a mix of web scraping and exploratory data analysis (EDA), we investigate differences in skincare products, price points and product formulation.

The goal is to demonstrate data wrangling, visualization, and storytelling skills while uncovering insights into skincare product trends.

---

## 📊 Problem Statement

> **How do Korean and Western skincare products differ in terms of price, formulation complexity, and consumer satisfaction?**

By analyzing ingredient density, product types, and pricing, we aim to inform data-driven skincare recommendations — and lay the groundwork for a future **AI-powered regimen builder**.

---

## 📁 Project Structure

```
skincare/
  ├── data/
  │   └── final_skincare_products.csv                    #final dataset for EDA
  │   └── skincare_full.csv                              #ignore
  │   ├── olive/
  │       ├── skincare_full.csv
  │   ├── sephora/
  │       ├── skincare_full.csv
  ├── notebooks/
  │   ├── 00_datascraping.ipynb                          # Scrapes ingredient + detail data from Olive Young
  │   ├── 01_data_cleaning_and_preparation.ipynb         # Cleans, filters, and preprocesses the dataset
  │   └── 02_eda_visualization.ipynb                     # Exploratory Data Analysis and insights
  ├── visualizations/
  │   └── plots
  ├── README.md

```

---

## 🧼 Data Scraping & Cleaning Highlights

- Sephora dataset obtained from Kaggle
- Olive Young dataset manually scraped using developer inspect tools and Python Selenium
- Removed products with missing or irrelevant ingredient info
- Filtered out rows with anomalous price or rating values
- Standardized product type categories
- Dropped non-functional placeholder ingredients (like `'1'`)

---

## 🔬 EDA Highlights

### 📦 Ingredient Trends
- Korean skincare features more **botanical and fermented ingredients** (e.g., centella, ginseng)
- Western skincare includes more **targeted actives** (e.g., retinol, peptides)

### ⭐ Ratings by Product Type
- **Essences and toners** are among the most consistently highly rated products
- Masks and serums show greater variability in satisfaction

### 💰 Pricing Patterns
- Western skincare is generally **more expensive** across product types
- Korean products provide more ingredients per dollar on average

### 🌡️ Ingredient Density
- Korean products tend to have **longer ingredient lists**, especially in categories like creams and ampoules
- Western brands lean toward **simplified formulas**

---

## 📌 Key Insights

- K-Beauty may offer **more accessible pricing** and **complex, layered formulations**
- Western products are positioned as **premium**, often with a narrower focus
- Consumers rate both categories highly, but K-Beauty has a slight edge in satisfaction
- Ingredient trends reflect deeper regional philosophies in skincare

---

## 🔮 Future Ideas

- 🤖 Build an **AI-powered skincare recommender**
- 🔍 Add ingredient **safety classification (e.g., EWG rating)**
- 📦 Cluster products by ingredient similarity or skin concerns
- 📈 Tableau or Streamlit app version (if time allows)

