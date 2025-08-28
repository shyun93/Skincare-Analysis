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

## 📊 Why?
Growing up with incredibly troubled skin, I've tried many products to help calm down my inflammation and acne. I'm particularly passionate about skincare and finding the best products to try and add to my self care regimen. As a Korean American, I wanted to specifically focus on Korean vs Western skincare products to maximize my options.

> **How do Korean and Western skincare products differ in terms of price, formulation complexity, and consumer satisfaction?**

By analyzing ingredient density, product types, and pricing, we aim to inform data-driven skincare recommendations — and lay the groundwork for a future **AI-powered regimen builder**.

---

## 📁 Project Structure

```
skincare/
  ├── data/
  │   └── final_skincare_products.csv                    #final cleaned dataset (olive & sephora combined) for EDA
  │   └── skincare_full.csv                              #ignore (realized there was 1 more cleaning to be done after I exported this)
  │   ├── olive/
  │       ├── oliveyoung_all_scraped_batches.csv         #scraped data using selenium
  │       ├── oliveyoung_sunscreen_scrapedv2.csv         #sunscreen data scraped separately 
  │       ├── oliveyoung_sunscreen_parsed.csv            #sunscreen data parsed from html from developer inspect tool
  │       ├── olive_cleaned.csv                          #cleaned olive young data
  │   ├── sephora/
  │       ├── product_info.csv                           #dataset obtained from Kaggle
  │       ├── sephora_cleaned.csv                        #cleaned sephora data
  ├── notebooks/
  │   ├── 00_datascraping.ipynb                          # Scrapes ingredient + detail data from Olive Young
  │   ├── 01_data_cleaning_and_preparation.ipynb         # Cleans, filters, and preprocesses the dataset
  │   └── 02_eda_visualization.ipynb                     # Exploratory Data Analysis and insights
  ├── visualizations/
  │   ├── ingredient_heat.png                            # ingredient heat map western vs k-beauty
  │   ├── Price_Product_Type.png                         # Price points of product types 
  │   ├── Product_Type_Region.png                        # Product Type count Western vs Korean 
  │   ├── Rating_Product_Type.png                        # Ratings of product types Western vs Korean 
  │   └── value_score.png                                # Box plot of value scores (rating/price)

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

- 🤖 Build an **AI-powered skincare recommender** - recommend potential ingredient combinations for additional customization
- 🔍 Add ingredient **safety classification (e.g., EWG rating)** (similar to Yuka)
- 📦 Cluster products by ingredient similarity or skin concerns
- 📈 Tableau or Streamlit app version (if time allows)

