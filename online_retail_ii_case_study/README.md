# Online Retail Data Analysis

## 📌 Project Overview
This project performs a comprehensive data analysis for a UK-based online retailer to identify key growth drivers and optimize inventory management. By analyzing over 540,000 transactions, the analysis uncovers seasonal trends, top-performing products, and high-potential international markets to support actionable business recommendations.

---

## 🛠️ Tech Stack

**Language**
- Python 3.x

**Libraries**
- Pandas — Data manipulation and cleaning  
- Matplotlib & Seaborn — Data visualization  
- NumPy — Numerical operations  

---

## 🚀 Data Analysis Phases

### 1. Act (Business Task)
**Problem:**  
Lack of visibility on seasonal sales trends, customer distribution, and international market performance leading to inventory inefficiencies.

**Objective:**  
Provide data-backed insights to increase revenue and effectively manage stock levels.

---

### 2. Prepare (Data Sourcing)
**Source:**  
UCI Machine Learning Repository (Online Retail II dataset)

**Structure:**  
8 columns including:
- Invoice Number  
- StockCode  
- Description  
- Quantity  
- InvoiceDate  
- Price  
- CustomerID  
- Country  

**Integrity:**  
Verified data using the ROCCC framework:
- Reliability  
- Originality  
- Comprehensiveness  
- Currency  
- Citation  

---

### 3. Process (Data Cleaning)

Cleaned the dataset to ensure high-quality analysis:

- **Handling Nulls:** Identified and removed 135,080 records missing Customer ID  
- **Anomaly Filtering:** Removed ~9,000 records containing negative quantities (returns) and zero-price adjustments  
- **Data Type Formatting:** Converted `InvoiceDate` to datetime and `CustomerID` to string to avoid mathematical errors  
- **Feature Engineering:** Created a `total_revenue` column (`Quantity × Price`) to enable financial analysis  

---

### 4. Analyse & Share (Data Insights)

Key findings discovered during exploration:

- **Seasonal Trends:** Revenue nearly doubles in Q4 (August–November), indicating a strong holiday peak  
- **Product Performance:** “Paper Craft Little Birdie” identified as the top revenue-generating item  
- **International Markets:** The UK remains the primary market, while the Netherlands and EIRE (Ireland) show strong expansion potential  
- **Daily Averages:** Average daily and monthly revenue benchmarks identified to detect underperforming periods  

---

## 💡 Recommendations

- **Holiday Inventory Scaling:** Increase stock levels for top products starting in late August to prepare for the Q4 surge  
- **Geo-Targeted Marketing:** Launch localized shipping promotions in the Netherlands and EIRE to capture untapped market share  
- **Customer Loyalty Program:** Implement an RFM (Recency, Frequency, Monetary) strategy to reward high-value customers and encourage purchases during off-peak months (February–April)  

---

## 📂 Project Structure

```plaintext
├── datasets/
│   ├── online_retail_II.csv        # Raw Data
│   └── processed/
│       └── cleaned_retail_data.csv # Final Cleaned Data
├── online_retail_II.ipynb          # Main Analysis Notebook
└── README.md                       # Project Documentation
## ⚙️ How to Run
Clone the repository
Ensure the online_retail_II.csv file is located in the datasets folder
Install dependencies:
```
pip install pandas matplotlib seaborn
```
Run the Jupyter Notebook:
online_retail_II.ipynb
