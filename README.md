# Data Warehouse and Analytics Project

**EN:** A modern SQL Server-based data warehouse project designed to integrate, transform, and model data for analytics and business reporting.  
**ID:** Proyek data warehouse modern berbasis SQL Server yang dirancang untuk mengintegrasikan, mentransformasi, dan memodelkan data untuk kebutuhan analisis dan pelaporan bisnis.

---

## Project Summary

**EN:** This project demonstrates an end-to-end data warehousing workflow, starting from raw data ingestion to business-ready analytical datasets. It applies industry-relevant practices in data engineering, ETL development, and analytical modeling.  
**ID:** Proyek ini menunjukkan alur kerja data warehouse secara end-to-end, mulai dari pemuatan data mentah hingga menjadi dataset analitis yang siap digunakan. Proyek ini menerapkan praktik yang relevan dalam data engineering, pengembangan ETL, dan pemodelan analitis.

---

## Architecture

**EN:** The warehouse is built using the Medallion Architecture with three layers: Bronze, Silver, and Gold.  
**ID:** Data warehouse ini dibangun menggunakan Arsitektur Medallion dengan tiga lapisan: Bronze, Silver, dan Gold.

- **Bronze**  
  **EN:** Stores raw data from source systems.  
  **ID:** Menyimpan data mentah dari sistem sumber.

- **Silver**  
  **EN:** Cleans, standardizes, and transforms the data.  
  **ID:** Membersihkan, menstandarisasi, dan mentransformasi data.

- **Gold**  
  **EN:** Provides business-ready data models for reporting and analytics.  
  **ID:** Menyediakan model data siap pakai untuk pelaporan dan analisis.

---

## Tech Stack

- **Database:** SQL Server Express  
- **Query Tool:** SQL Server Management Studio (SSMS)  
- **Design Tool:** Draw.io  
- **Version Control:** GitHub  

---

## Key Features

- **EN:** Build ETL pipelines from ERP and CRM source systems  
  **ID:** Membangun pipeline ETL dari sistem sumber ERP dan CRM

- **EN:** Transform raw data into clean and structured analytical datasets  
  **ID:** Mengubah data mentah menjadi dataset analitis yang bersih dan terstruktur

- **EN:** Design fact tables and dimension tables for analytical querying  
  **ID:** Merancang fact table dan dimension table untuk kebutuhan query analitis

- **EN:** Generate SQL-based reports for business insight generation  
  **ID:** Menghasilkan laporan berbasis SQL untuk menghasilkan insight bisnis

- **EN:** Analyze customer behavior, product performance, and sales trends  
  **ID:** Menganalisis perilaku pelanggan, kinerja produk, dan tren penjualan

---

## Project Workflow

**EN:** The workflow of this project can be summarized as follows:  
**ID:** Alur kerja proyek ini dapat diringkas sebagai berikut:

1. **EN:** Extract raw data from ERP and CRM source files  
   **ID:** Mengambil data mentah dari file sumber ERP dan CRM

2. **EN:** Load raw data into the Bronze layer  
   **ID:** Memuat data mentah ke lapisan Bronze

3. **EN:** Clean and transform data in the Silver layer  
   **ID:** Membersihkan dan mentransformasi data di lapisan Silver

4. **EN:** Build analytical models in the Gold layer  
   **ID:** Membangun model analitis di lapisan Gold

5. **EN:** Perform SQL-based analysis and reporting  
   **ID:** Melakukan analisis dan pelaporan berbasis SQL

---

## Analytics Focus

**EN:** This project focuses on three main analytical areas:  
**ID:** Proyek ini berfokus pada tiga area analisis utama:

- **Customer Behavior**  
- **Product Performance**  
- **Sales Trends**

---

## Repository Structure

```bash
data-warehouse-project/
├── datasets/          # Raw datasets from ERP and CRM
├── docs/              # Documentation and architecture files
├── scripts/           # SQL scripts for ETL and transformations
│   ├── bronze/
│   ├── silver/
│   └── gold/
├── tests/             # Testing and validation files
├── README.md
└── LICENSE
```

---

## Portfolio Value

**EN:** This project highlights practical skills in SQL Development, Data Engineering, ETL Pipeline Development, Data Modeling, and Data Analytics. It also demonstrates an end-to-end understanding of how raw data is transformed into actionable business insights.  
**ID:** Proyek ini menampilkan kemampuan praktis dalam SQL Development, Data Engineering, ETL Pipeline Development, Data Modeling, dan Data Analytics. Selain itu, proyek ini juga menunjukkan pemahaman end-to-end tentang bagaimana data mentah diolah menjadi insight bisnis yang dapat digunakan.

---

## License

**EN:** This project is licensed under the MIT License.  
**ID:** Proyek ini menggunakan Lisensi MIT.
