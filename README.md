# 📦 SQL Data Warehouse Project
This project demonstrates the end-to-end development of a SQL-based Data Warehouse using a multi-layered architecture (Bronze, Silver, Gold). It includes source analysis, schema design, ETL pipeline development, data modeling, and documentation.

## 📁 Project Structure

      ### 🔷 Bronze Layer
            - **Source System Analysis**  
            - **Create Database & Schemas**
            - **DDL for Tables**
            - **Develop SQL Load Scripts**
            - **Stored Procedures for Data Load**
            - **Document Data Flow**
            
            ### ⚙️ Tasks
            - Prepare Git Repository
            - Create & Commit Code
            - Build Bronze Layer
      
      ### 🔘 Silver Layer
          - **Explore & Understand the Data**
          - **Create DDL for Tables**
          - **Clean & Load Data into Staging**
            - CRM: `crm_cust_info`, `crm_prd_info`, `crm_sales_details`
            - ERP: `erp_cust_az12`, `erp_loc_a101`, `erp_px_cat_g1v2`
          - **Stored Procedures**
          - **Document Data Flow**
      
      ### 🟡 Gold Layer
          - **Business Understanding**
          - **Data Modeling Concepts**
            - Star Schema vs. Snowflake Schema
            - Dimensions vs. Facts
          - **Create Dimension & Fact Tables**
            - Customers, Products, Sales
          - **Build Final Star Schema Model**
          - **Data Catalog & Final Flow Documentation**

## 📌 Key Concepts Covered
- Data Warehouse Layering (Bronze → Silver → Gold)
- Schema Design & SQL DDL
- ETL Development with SQL Scripts & Stored Procedures
- Data Modeling (Star vs Snowflake)
- Dimension & Fact Table Design
- Data Flow Documentation

## 🛠 Tools & Technologies
- SQL (Any RDBMS: SQL Server, PostgreSQL, Snowflake, etc.)
- Git & GitHub for Version Control
- Data Modeling Techniques

## ✅ How to Use
1. Clone the repository.
2. Review SQL scripts and documentation in each layer's folder.
3. Follow the README steps in order for a complete walkthrough.
4. Modify scripts for your own data sources and schema if needed.

## 📄 License
This project is for educational and demonstration purposes.
