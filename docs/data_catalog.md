# Data Catalog for Gold Layer | Katalog Data untuk Gold Layer

## Overview | Gambaran Umum

**EN:**  
The **Gold Layer** represents the business-level data model designed to support reporting and analytical use cases. It consists of **dimension tables** and **fact tables** that provide clean, enriched, and business-ready data for decision-making.

**ID:**  
**Gold Layer** merepresentasikan model data tingkat bisnis yang dirancang untuk mendukung kebutuhan pelaporan dan analisis. Layer ini terdiri dari **tabel dimensi** dan **tabel fakta** yang menyediakan data bersih, kaya informasi, dan siap digunakan untuk pengambilan keputusan.

---

## 1. `gold.dim_customers`

**Purpose | Tujuan**

**EN:** Stores customer information enriched with demographic and geographic attributes.  
**ID:** Menyimpan informasi pelanggan yang telah diperkaya dengan atribut demografis dan geografis.

### Columns | Kolom

| Column Name | Data Type | EN | ID |
|-------------|-----------|----|----|
| customer_key | INT | Surrogate key that uniquely identifies each customer record in the dimension table. | Surrogate key yang secara unik mengidentifikasi setiap record pelanggan pada tabel dimensi. |
| customer_id | INT | Unique numeric identifier assigned to each customer. | Identitas numerik unik yang diberikan kepada setiap pelanggan. |
| customer_number | NVARCHAR(50) | Alphanumeric customer identifier used for tracking and reference. | Identitas alfanumerik pelanggan yang digunakan untuk pelacakan dan referensi. |
| first_name | NVARCHAR(50) | Customer's first name. | Nama depan pelanggan. |
| last_name | NVARCHAR(50) | Customer's last name or family name. | Nama belakang atau nama keluarga pelanggan. |
| country | NVARCHAR(50) | Customer's country of residence (e.g., `Australia`). | Negara tempat tinggal pelanggan (misalnya, `Australia`). |
| marital_status | NVARCHAR(50) | Customer's marital status (e.g., `Married`, `Single`). | Status pernikahan pelanggan (misalnya, `Married`, `Single`). |
| gender | NVARCHAR(50) | Customer's gender (e.g., `Male`, `Female`, `N/A`). | Jenis kelamin pelanggan (misalnya, `Male`, `Female`, `N/A`). |
| birthdate | DATE | Customer's date of birth in `YYYY-MM-DD` format. | Tanggal lahir pelanggan dalam format `YYYY-MM-DD`. |
| create_date | DATE | Date when the customer record was created in the source system. | Tanggal saat data pelanggan dibuat di sistem sumber. |

---

## 2. `gold.dim_products`

**Purpose | Tujuan**

**EN:** Provides product details and related attributes for analytical use.  
**ID:** Menyediakan detail produk dan atribut terkait untuk kebutuhan analisis.

### Columns | Kolom

| Column Name | Data Type | EN | ID |
|-------------|-----------|----|----|
| product_key | INT | Surrogate key that uniquely identifies each product record in the dimension table. | Surrogate key yang secara unik mengidentifikasi setiap record produk pada tabel dimensi. |
| product_id | INT | Unique identifier assigned to the product for internal reference. | Identitas unik yang diberikan kepada produk untuk referensi internal. |
| product_number | NVARCHAR(50) | Structured alphanumeric code representing the product. | Kode alfanumerik terstruktur yang merepresentasikan produk. |
| product_name | NVARCHAR(50) | Descriptive product name, including type, color, and size details. | Nama produk yang bersifat deskriptif, termasuk tipe, warna, dan ukuran. |
| category_id | NVARCHAR(50) | Unique identifier for the product category. | Identitas unik untuk kategori produk. |
| category | NVARCHAR(50) | High-level product classification (e.g., `Bikes`, `Components`). | Klasifikasi tingkat tinggi untuk produk (misalnya, `Bikes`, `Components`). |
| subcategory | NVARCHAR(50) | More detailed classification within the product category. | Klasifikasi yang lebih rinci di dalam kategori produk. |
| maintenance_required | NVARCHAR(50) | Indicates whether the product requires maintenance (e.g., `Yes`, `No`). | Menunjukkan apakah produk memerlukan perawatan (misalnya, `Yes`, `No`). |
| cost | INT | Cost or base price of the product in whole currency units. | Biaya atau harga dasar produk dalam satuan mata uang penuh. |
| product_line | NVARCHAR(50) | Product line or series (e.g., `Road`, `Mountain`). | Lini atau seri produk (misalnya, `Road`, `Mountain`). |
| start_date | DATE | Date when the product became available for sale or use. | Tanggal saat produk mulai tersedia untuk dijual atau digunakan. |

---

## 3. `gold.fact_sales`

**Purpose | Tujuan**

**EN:** Stores transactional sales data for reporting and business analysis.  
**ID:** Menyimpan data transaksi penjualan untuk kebutuhan pelaporan dan analisis bisnis.

### Columns | Kolom

| Column Name | Data Type | EN | ID |
|-------------|-----------|----|----|
| order_number | NVARCHAR(50) | Unique alphanumeric identifier for each sales order (e.g., `SO54496`). | Identitas alfanumerik unik untuk setiap pesanan penjualan (misalnya, `SO54496`). |
| product_key | INT | Surrogate key linking the transaction to the product dimension. | Surrogate key yang menghubungkan transaksi ke dimensi produk. |
| customer_key | INT | Surrogate key linking the transaction to the customer dimension. | Surrogate key yang menghubungkan transaksi ke dimensi pelanggan. |
| order_date | DATE | Date when the order was placed. | Tanggal saat pesanan dibuat. |
| shipping_date | DATE | Date when the order was shipped. | Tanggal saat pesanan dikirim. |
| due_date | DATE | Date when the payment was due. | Tanggal jatuh tempo pembayaran. |
| sales_amount | INT | Total sales value for the line item in whole currency units. | Total nilai penjualan untuk setiap baris transaksi dalam satuan mata uang penuh. |
| quantity | INT | Number of product units ordered in the line item. | Jumlah unit produk yang dipesan pada baris transaksi. |
| price | INT | Unit price of the product in whole currency units. | Harga per unit produk dalam satuan mata uang penuh. |

---

## Notes | Catatan

**EN:**  
- The **dimension tables** (`dim_customers` and `dim_products`) provide descriptive business context.  
- The **fact table** (`fact_sales`) stores measurable transactional data.  
- Together, these tables form a **star schema** that supports analytics, dashboards, and reporting.

**ID:**  
- **Tabel dimensi** (`dim_customers` dan `dim_products`) menyediakan konteks bisnis yang bersifat deskriptif.  
- **Tabel fakta** (`fact_sales`) menyimpan data transaksi yang dapat diukur.  
- Secara keseluruhan, tabel-tabel ini membentuk **star schema** yang mendukung analisis, dashboard, dan pelaporan.
