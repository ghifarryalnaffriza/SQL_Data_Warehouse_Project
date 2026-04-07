# Data Source Relationship Overview

![Data Source Relationship Overview](docs/Hubungan%20antar%20tabel.jpg)

## Description
This diagram illustrates the relationships between source tables from the CRM and ERP systems used in the data warehouse project. It shows how sales, customer, product, category, and location data are connected before going through the ETL and data modeling process.

## Penjelasan
Diagram ini menggambarkan hubungan antar tabel sumber dari sistem CRM dan ERP yang digunakan dalam proyek data warehouse. Diagram ini menunjukkan bagaimana data penjualan, pelanggan, produk, kategori, dan lokasi saling terhubung sebelum masuk ke proses ETL dan pemodelan data.

---

## Table Relationships

### 1. `crm_sales_detail` → `crm_prd_info`
- **EN:** Connected through `prd_key` to link each sales transaction with product information.
- **ID:** Terhubung melalui `prd_key` untuk mengaitkan setiap transaksi penjualan dengan informasi produk.

### 2. `crm_sales_detail` → `crm_cus_info`
- **EN:** Connected through `cst_id` to associate each sales record with customer details.
- **ID:** Terhubung melalui `cst_id` untuk menghubungkan setiap data penjualan dengan detail pelanggan.

### 3. `crm_prd_info` → `erp_px_cat`
- **EN:** Connected to enrich product data with category and subcategory information.
- **ID:** Terhubung untuk memperkaya data produk dengan informasi kategori dan subkategori.

### 4. `crm_cus_info` → `erp_cust_az12`
- **EN:** Connected to enrich customer data with additional demographic attributes.
- **ID:** Terhubung untuk memperkaya data pelanggan dengan atribut demografis tambahan.

### 5. `crm_cus_info` → `erp_loc_a101`
- **EN:** Connected to add customer location or country information.
- **ID:** Terhubung untuk menambahkan informasi lokasi atau negara pelanggan.

---

## Purpose

- **EN:** This relationship mapping helps define how source data is integrated and transformed into the Bronze, Silver, and Gold layers of the data warehouse.
- **ID:** Pemetaan relasi ini membantu menentukan bagaimana data sumber diintegrasikan dan ditransformasikan ke dalam layer Bronze, Silver, dan Gold pada data warehouse.

- **EN:** It also serves as a reference for building joins, transformations, and analytical models.
- **ID:** Diagram ini juga berfungsi sebagai acuan dalam membangun proses join, transformasi, dan model analitis.
