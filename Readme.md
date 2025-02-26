# Global Retail Daily Sales Data Flow


Bronze Tables:

Data are automated to upload from DBFS in CSV, JSON and Parquet format contain customer, products and orders data.

** Backup data are automaed to be saved in Archive directory with current date suffix file's names


Silver Tables:

1- perform incremental data ingestion through creating view tables

2- Perform Data normalization, data cleaning and create customer segmentation, stock calculation, price category and stock status calculation.

3- Utilized Merge and insert to update and upload new values into silver table and avoid duplication


Gold Tables:

Two Gold tables are resulted as final outputs:

1- Goldlayer_dailysales by category ==> created through joining Product and order silver tables

2- Goldlayer_dailysales ==> created through joining Product and Customer silver tables




![image](https://github.com/user-attachments/assets/bf2a55e4-f35b-4a6e-888b-d160cb8b699a)

