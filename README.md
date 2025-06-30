# 🛒 Market Basket Analysis for Tech Retail
Market Basket Analysis using Apriori for a tech retail dataset to identify cross-sell opportunities, using Python and data visualization.


This project uses **Market Basket Analysis with the Apriori algorithm** on a simulated **tech retail environment dataset** to identify **cross-sell opportunities** and actionable business strategies for maximizing basket value in retail.

---

## 🚀 Project Overview

Retailers handle vast numbers of transactions daily but may miss hidden product purchase patterns that can increase revenue and customer satisfaction.

Using Market Basket Analysis:
✅ We identify **frequent itemsets** (high-demand products)  
✅ Discover **strong association rules with high lift and confidence**  
✅ Recommend **data-driven bundling and cross-sell strategies**

---

## 🗂️ Project Structure

- `notebooks/` – Clean Google Colab notebook with step-by-step analysis
- `data/` – Cleaned dataset (`tech_market_basket.csv`) for analysis
- `images/` – Visualizations for quick reference
- `requirements.txt` – Python dependencies

---

## 🛠️ Tools & Libraries

- Python: `pandas`, `numpy`
- Data Visualization: `matplotlib`, `seaborn`
- Association Rule Mining: `mlxtend`

---

## 📊 Key Steps

✅ **Data Cleaning & Preprocessing**  
✅ **EDA with Product Distribution Visualization**  
✅ **Apriori Algorithm for Frequent Itemsets**  
✅ **Association Rule Mining with Support, Confidence, Lift**  
✅ **Visualizations (bar plots, lift analysis)**

---

## 📈 Key Findings

From analyzing **~12,000 transactions with realistic co-purchase patterns**:

### 1️⃣ Frequent Itemsets
- **Smartphone Case – Silicone (27% support)**, **Smartphone – XPhone 12 (18.5%)**, and **Over-Ear Headphones – BassBoost (17.7%)** were among the **most frequently purchased items**, indicating high customer interest and ensuring these should remain stocked and prioritized in promotions.

### 2️⃣ Association Rules with High Lift & Confidence

| Antecedents | Consequents | Support | Confidence | Lift |
|-------------|-------------|---------|------------|------|
| (Smartphone Case, VR Headset) | Bluetooth Speaker | 1.25% | 73% | 4.61 |
| (VR Headset) | (Bluetooth Speaker, Smartphone Case) | 1.25% | 43% | 4.80 |
| (Game Controller, Over-Ear Headphones) | Gaming Console | 1.08% | 52% | 4.58 |

**Interpretation:**
- Customers buying a **VR Headset are 4.8x more likely to also buy a Bluetooth Speaker and Smartphone Case**.
- **Game Controller + Over-Ear Headphones buyers are 4.6x more likely to buy a Gaming Console**.
- High-confidence cross-sell patterns (up to **73%**) present clear opportunities to **increase basket size through bundling**.

---

## 💡 Business Recommendations

✅ **Cross-Sell Strategies:**
- Bundle **VR Headsets + Bluetooth Speakers + Smartphone Cases**.
- Bundle **Gaming Consoles with Controllers and Headphones**.
- Recommend **Laptop Sleeve and USB-C Charger** during laptop purchases.

✅ **Promotions:**
- "Frequently Bought Together" discounts for identified pairs.
- Targeted follow-up emails offering accessories related to recent purchases.

✅ **Store Layout Optimization:**
- Place frequently associated products nearby for seamless physical cross-selling.

---

## 📂 Running the Project

1️⃣ Clone this repository:
```bash
git clone https://github.com/YOUR_USERNAME/market-basket-analysis-tech-retail.git
cd market-basket-analysis-tech-retail
