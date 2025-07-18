# 🟦 Bronze Layer – Raw Data Ingestion
This folder contains the scripts and procedures used to **load raw data into the Bronze Layer** of the Data Warehouse. The Bronze Layer acts as the **staging area**, storing untransformed data exactly as received from source systems (CRM and ERP).
---
## ⚙️ What `load_bronze.sql` Does
The `bronze.load_bronze` stored procedure:
- 🔄 **Truncates** old data from Bronze tables
- ⬇️ **Loads fresh CSV data** using `BULK INSERT`
- 🧾 **Logs duration** of each load operation
- 🧯 **Handles errors** gracefully using `TRY...CATCH`
- 📈 Prints total load time for monitoring and debugging
---
## 📥 Source Tables Loaded
| Source System | Table Name                  | CSV Path                                                  |
|---------------|-----------------------------|-----------------------------------------------------------|
| CRM           | `crm_cust_info`             | `datasets/source_crm/cust_info.csv`                       |
| CRM           | `crm_prd_info`              | `datasets/source_crm/prd_info.csv`                        |
| CRM           | `crm_sales_details`         | `datasets/source_crm/sales_details.csv`                   |
| ERP           | `erp_loc_a101`              | `datasets/source_erp/loc_a101.csv`                        |
| ERP           | `erp_cust_az12`             | `datasets/source_erp/cust_az12.csv`                       |
| ERP           | `erp_px_cat_g1v2`           | `datasets/source_erp/px_cat_g1v2.csv`                     |
> 📂 Make sure these CSV files are accessible to your SQL Server (e.g., correct drive path, network share, or local disk).
---
## ▶️ How to Run
1. Ensure all Bronze layer tables are created.
2. Update file paths in `load_bronze.sql` if needed.
3. Execute the procedure:
   ```sql
   EXEC bronze.load_bronze;
