# customer-purchase-data-pipeline
creating a project using pyspark and databricks
#Project Overview
## 📖 Overview
This project builds an end-to-end data pipeline to analyze customer purchase behavior using an e-commerce dataset.

The pipeline includes data ingestion, cleaning, transformation, aggregation, and storage using PySpark.
## 📊 Dataset
The dataset contains customer purchase data for 1 year in an American e-commerce platform.

### Key Columns:
- Order_Date: Order date
- Customer_id: Unique customer ID
- Product_Category: Category of product
- Sales: Total sales amount
- Quantity: Number of items purchased
- Discount: Discount applied
- Profit: Profit earned
- Shipping_cost: Delivery cost
- Device_Type: Web/Mobile usage
- Payment_method: Payment type
 ## 🏗 Architecture
   -Raw Data → PySpark Processing → Transformation → Aggregation →  Output is saved to table
## ⚙️ Tech Stack
- PySpark
- Python
- SQL
- Databricks
  
## 🔄 Pipeline Steps
1. Data Ingestion – Loaded CSV data using PySpark
2. Data Cleaning – Removed nulls and duplicates
3. Transformation – Created new columns like Final_Sales and Net_Profit
4. Aggregation – Generated KPIs such as sales by category and top customers
5. Storage –the output is stored in tables using saveAsTable 
##Output
   The transformed data and KPIs are stored as Delta tables in Databricks for efficient querying and analysis.
   --Tables Created:
      1.sales_category
      2.topcustomers
      3.sales_device
      4.deliveryanalysis
      5.profit_category
      6.totalrevenue
## 📈 Key Insights

- Identified top customers based on total spending
- Analyzed sales distribution across product categories
- Compared performance across device types
- Evaluated profit after shipping costs
