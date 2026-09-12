# Power BI Data Modeling Project

## Project Overview

This project demonstrates the process of transforming a **raw and complex Power BI data model into a clean, structured, and scalable analytical model**.

The primary objective was to understand the source data, identify business entities and events, define the correct grain, build dimensions and fact tables, establish appropriate relationships, and prepare the model for reliable reporting and analysis.

---

# Project Objective

The key objective of this project was to build a **clean Star Schema data model** that provides:

- Better data organization
- Reduced duplication
- Consistent relationships
- Accurate calculations
- Improved report performance
- Easier maintenance and scalability

---

# Data Modeling Process

The project followed a structured four-phase approach:

### **Phase 1 — Prepare & Explore**
- Imported and reviewed the source tables
- Understood the business process and available data
- Inspected tables, columns, keys, and relationships
- Identified potential dimensions and facts
- Cleaned and standardized the source data

### **Phase 2 — Build Dimensions**
- Grouped tables belonging to the same business entity
- Combined related tables where appropriate
- Removed unnecessary columns
- Validated uniqueness and cardinality
- Created standardized dimension tables

### **Phase 3 — Build Facts**
- Defined the grain before creating fact tables
- Used detailed transactional data as the fact foundation
- Added required dimension keys
- Validated measures before and after transformations
- Avoided unnecessary pre-aggregation
- Prevented direct Fact-to-Fact relationships

### **Phase 4 — Polish the Model**
- Applied naming and modeling standards
- Created a shared Date Dimension
- Organized measures into a dedicated measure table
- Implemented Row-Level Security (RLS)
- Validated relationships, measures, totals, and key business numbers

---

# Final Data Model

The final model follows a **Star Schema architecture**, where centralized fact tables connect to shared dimension tables.

### **Key Dimensions**

- `dim_customer`
- `dim_product`
- `dim_geo`
- `dim_date`
- `dim_campaign`
- `dim_order_flags`

### **Key Fact Tables**

- `fact_sales`
- `fact_inventory`
- `fact_order_process`
- `fact_campaign_spend`
- `fact_sales_target`
- `fact_promotion_coverage`

### **Supporting Tables**

- `security`
- `Measure`

---

# Key Modeling Practices

- **Defined the grain before building facts**
- **Validated dimension uniqueness**
- **Checked relationship cardinality**
- **Used shared dimensions across multiple facts**
- **Avoided direct Fact-to-Fact relationships**
- **Separated descriptive attributes from transactional events**
- **Reduced unnecessary duplication**
- **Validated numbers before and after major transformations**
- **Applied consistent naming conventions**
- **Created a centralized Date Dimension**
- **Implemented and tested RLS**

---

# Business Value

The cleaned model provides a strong foundation for building reliable Power BI reports and enables analysis across:

- Sales
- Customers
- Products
- Inventory
- Campaigns
- Promotions
- Order Processing
- Sales Targets
- Geographic Regions

The resulting model is **more organized, maintainable, scalable, and suitable for enterprise-level Power BI reporting**.

---

# Tools Used

- **Power BI Desktop**
- **Power Query**
- **DAX**
- **Data Modeling**
- **Star Schema**
- **Row-Level Security (RLS)**

---

# Project Highlights

✔ Raw Model → Cleaned Model  
✔ Star Schema Data Modeling  
✔ Fact & Dimension Design  
✔ Grain Definition  
✔ Relationship & Cardinality Validation  
✔ Data Transformation & Standardization  
✔ Date Dimension  
✔ DAX Measures  
✔ Row-Level Security  
✔ Final Model Validation  

---

# Modeling Flow

**Explore → Clean → Transform → Combine → Build Dimensions → Define Grain → Build Facts → Validate → Standardize → Date → Measures → RLS → Test → Star Schema**

# Author
## Amit Kumar
## Data Analyst
