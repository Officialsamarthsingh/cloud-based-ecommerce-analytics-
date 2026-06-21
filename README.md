# Cloud-Based E-commerce Analytics

### Project Overview

This project demonstrates an end-to-end cloud-based analytics workflow using Python, AWS, SQL, and Power BI. The objective was to transform raw e-commerce transaction data into actionable business insights through data cleaning, exploratory analysis, cloud storage, SQL-based querying, and interactive dashboarding.

The project follows a realistic analytics pipeline, beginning with data preparation and ending with business-focused reporting and recommendations.

---

### Business Problem

E-commerce businesses generate large volumes of transactional data across customers, products, and orders. The challenge is to convert this data into meaningful insights that support decision-making.

This project aims to answer questions such as:

- Which product categories drive the most revenue and profit?
- Which customer segments contribute the highest value?
- How do sales trends change over time?
- Which categories experience the highest return rates?
- How does business performance vary across regions?

---

### Project Architecture

Raw Dataset
→ Data Cleaning & Validation (Python)
→ Exploratory Data Analysis (Google Colab)
→ Data Modeling (Customers, Products, Orders)
→ AWS S3 Storage
→ Amazon Athena SQL Analysis
→ Power BI Data Modeling & Dashboarding
→ Business Presentation & Recommendations

---

### Dataset

The dataset contains e-commerce transaction records including:

- Customer Information
- Product Information
- Order Details
- Revenue Metrics
- Profitability Metrics
- Shipping Information
- Product Returns

---

### Data Preparation

The data preparation process included:

- Missing value assessment
- Duplicate record validation
- Customer and product attribute consistency checks
- Data type corrections
- Feature engineering
- Customer age-group segmentation

A "Latest Record Wins" approach was used to resolve conflicting customer and product attributes.

---

### Data Modeling

To support scalable analytics and SQL querying, the dataset was transformed into three relational tables:

Customers

- Customer ID
- Age
- Gender
- Region

Products

- Product ID
- Category
- Price
- Profit Margin

Orders

- Order ID
- Customer ID
- Product ID
- Order Date
- Quantity
- Total Amount
- Payment Method
- Shipping Cost
- Delivery Time
- Return Status

---

### AWS & SQL Analysis

The modeled datasets were uploaded to Amazon S3 and queried using Amazon Athena.

Analysis included:

- Revenue Analysis
- Customer Analysis
- Regional Performance Analysis
- Category Performance Analysis
- Return Rate Analysis
- Profitability Analysis

SQL techniques used:

- Joins
- Aggregations
- Common Table Expressions (CTEs)
- Window Functions
- Ranking Functions
- Conditional Logic

---

### Dashboard Development

Interactive dashboards were developed in Power BI covering:

Executive Overview

- Revenue Performance
- Order Trends
- Regional Analysis

Customer Analytics

- Customer Demographics
- Revenue Contribution
- Top Customers

Product Analytics

- Revenue by Category
- Profitability Analysis
- Return Analysis

Operations Analytics

- Delivery Performance
- Shipping Cost Analysis
- Return Behavior

---

### Key Insights

- Revenue was concentrated within a small number of product categories.
- A limited group of customers contributed a significant share of total revenue.
- Return rates varied considerably across categories, impacting profitability.
- Regional performance differences highlighted opportunities for targeted growth.
- Product profitability did not always align with revenue performance.

---

### Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Amazon S3
- Amazon Athena
- SQL
- Power BI

---

### Repository Structure

├── data/
├── notebooks/
│   └── EDA.ipynb
├── aws/
│   ├── s3_bucket_structure.png
│   ├── athena_tables.png
│   └── athena_query_results.png
├── dashboard/
│   └── PowerBI.pbix
│   └── images/
│    ├── data_model.png
│    ├── executive_dashboard.png
│    ├── customer_dashboard.png
│    ├── product_dashboard.png
│    └── operations_dashboard.png
├── presentation/
│   └── Project_Presentation.pdf
└── README.md

---

### Author

Samarth Gupta

Aspiring Data Analyst with interests in data analytics, business intelligence, cloud analytics, and machine learning.
