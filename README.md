# 🪑 E-commerce Furniture Dataset 2024 - Sales Prediction Project

This project analyzes and predicts sales of furniture products listed on an e-commerce platform (AliExpress) using machine learning and exploratory data analysis. The dataset includes 2,000 entries containing product details, prices, and sales metrics.

---

## 📌 Objective

To predict the number of items sold (sold) based on product attributes such as:

- Product title
- Price
- Tag text (e.g., "Free shipping")

---

## 📊 Dataset Overview

- *Source:* Scraped from AliExpress using Apify
- *Entries:* 2,000 furniture products
- *Columns:*
  - productTitle: Name of the furniture item
  - originalPrice: Original price before discount (dropped due to missing values)
  - price: Final price
  - sold: Number of units sold
  - tagText: Tags such as shipping info

> 📁 Dataset File: ecommerce_furniture_dataset_2024.csv

---

## ⚙️ Tech Stack

- Python 3
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- TF-IDF Vectorizer

---

## 🔍 Project Workflow

1. *Data Loading*  
   Load and inspect the CSV dataset.

2. *Data Preprocessing*  
   - Drop irrelevant or null-heavy columns (originalPrice)
   - Clean price column and convert to float
   - Simplify and encode tagText

3. *Exploratory Data Analysis (EDA)*  
   - Price and Sold distribution plots
   - Scatter plot of price vs sold
   - Pair plots for tag-based filtering

4. *Feature Engineering*  
   - TF-IDF Vectorization of productTitle

5. *Model Building*  
   - Linear Regression
   - Random Forest Regressor

6. *Model Evaluation*  
   - Mean Squared Error (MSE)
   - R² Score

---

## 📈 Results

| Model              | MSE (↓)     | R² Score (↑) |
|-------------------|-------------|--------------|
| Linear Regression | e.g., 103 | e.g., 0.51 |
| Random Forest     | e.g., 64  | e.g., 0.73 |

> 🔍 *Note:* Random Forest gave better performance on unseen test data.

---

## 🚀 How to Run

1. *Clone the repository*:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
