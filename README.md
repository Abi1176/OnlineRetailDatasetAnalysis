**Dataset Overview**

This dataset contains transaction records of a UK-based online retailer from 2010 to 2011.This analyzes the Online Retail Dataset from the UCI Machine Learning Repository to uncover customer purchasing patterns, best-selling products, and segmentation insights using unsupervised learning techniques. 

🔗 **Dataset Source:** [UCI Machine Learning Repository - Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

**Data Size: 541,909 transactions**

**Time Period: 2010-2011**

**Columns:**

    **InvoiceNo:** Unique identifier for each transaction
    
    **StockCode:** Unique identifier for each product
    
    **Description:** Product name
    
    **Quantity:** Number of products purchased
    
    **InvoiceDate**: Date of purchase
    
    **UnitPrice**: Price per item
    
    **CustomerID:** Unique identifier for each customer
    
    **Country:** Country of the customer

**Data Preprocessing & Cleaning**

    🔹Removed missing values and duplicate records
    
    🔹Filtered out canceled transactions (negative quantities)
    
    🔹Created a TotalPrice column (Quantity × UnitPrice)

**Exploratory Data Analysis (EDA)**

**Key Insights from Data Exploration**:

    🔹The dataset contains 4,373 unique customers.
    
    🔹Top-selling products: Seasonal gifts and home décor dominate sales.
    
    🔹Peak sales months: November and December show the highest transactions (holiday shopping effect).
    
    🔹Geographical trends: The UK contributes 85% of total sales, while Germany and France are also key markets.

**Sales Distribution by Country:**

**Country	Percentage of Sales**

    🔹United Kingdom	85%
    
    🔹Germany	2.5%
    
    🔹France	2.3%
    
    🔹Others	10.2%

**Customer Segmentation Using RFM Analysis**

For customer segmentation we use Recency, Frequency, and Monetary (RFM) Analysis to segment customers:

  **🔹Recency (R)**: How recently a customer made a purchase
  
  **🔹Frequency (F)**: How often a customer buys
  
  **🔹Monetary (M)**: How much a customer spends

**K-Means Clustering:**
  
  Using this algorithm customers were categorized into:
  
 **🔹High-Value Buyers** – Frequent, high-spending customers
 
 **🔹Occasional Buyers** – Moderate spending & purchase frequency
 
 **🔹One-Time Shoppers** – Rare purchases, low spending
 
 **🔹Lost Customers**– Haven’t purchased recently

**Conclusion**

**Business Recommendations**

Implement personalized marketing campaigns for high-value customers

Offer discounts & promotions to re-engage lost customers

Optimize inventory planning based on seasonal trends

**Future Work**

Predict future sales trends using Time-Series Forecasting

Conduct Market Basket Analysis to understand frequently bought-together products





