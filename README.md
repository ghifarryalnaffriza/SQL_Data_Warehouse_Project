---
# README English Version
---
# Data Warehouse and Analytics Project

Welcome to the **Data Warehouse and Analytics Project** repository.  
This project demonstrates the implementation of a **modern data warehouse** using **SQL Server**, covering the full workflow from data integration to analytics in order to generate insights that support business decision-making. It is also designed as a portfolio project to showcase practical skills in **data engineering** and **data analytics**.

---

## Project Overview

This project focuses on building a centralized data warehouse that integrates data from multiple source systems. The workflow includes:

- Extracting data from source systems
- Cleaning and transforming raw data
- Designing analytical data models
- Creating SQL-based analysis and reporting

The final output is a business-ready data model that can be used for reporting, dashboards, and analytical purposes.

---

## Data Architecture

This project follows the **Medallion Architecture**, which is divided into three main layers:

### Bronze Layer
This layer stores raw data from source systems in its original form. Data is loaded from CSV files into SQL Server with minimal modification.

### Silver Layer
This layer is responsible for data cleansing, standardization, and normalization to improve data quality and consistency.

### Gold Layer
This layer contains processed and business-ready data models prepared for reporting, dashboarding, and analytics.

---

## Project Scope

The scope of this project includes:

1. **Data Architecture Design**  
   Building a modern layered data warehouse using the Bronze, Silver, and Gold approach.

2. **ETL Pipelines**  
   Extracting, transforming, and loading data from source systems into the warehouse.

3. **Data Modeling**  
   Developing **fact tables** and **dimension tables** optimized for analytical queries.

4. **Analytics and Reporting**  
   Creating SQL-based analysis and reports to deliver actionable insights for stakeholders.

---

## Project Objective

The main objective of this project is to build a modern data warehouse using SQL Server to consolidate sales data from multiple sources for more effective reporting and analysis.

More specifically, the project aims to:

- Import data from two source systems: **ERP** and **CRM**
- Clean and resolve data quality issues before analysis
- Combine the data into an integrated and user-friendly analytical model
- Provide clear documentation to support both business and analytics needs

> Note: This project focuses only on the latest dataset and does not include historical data tracking.

---

## Analytics Focus

The analytical focus of this project is centered on three key areas:

- **Customer Behavior**
- **Product Performance**
- **Sales Trends**

Through SQL-based analytics, this project aims to generate insights that support business evaluation and better decision-making.

---

## Tools Used

The main tools used in this project include:

- **SQL Server Express** — database engine for storing and managing data
- **SQL Server Management Studio (SSMS)** — tool for database management and query execution
- **Draw.io** — for designing architecture diagrams, data flows, and data models
- **GitHub** — for version control and project documentation

---

## Repository Structure

```bash
data-warehouse-project/
│
├── datasets/                           # Raw datasets from ERP and CRM systems
│
├── docs/                               # Project documentation and architecture files
│   ├── etl.drawio
│   ├── data_architecture.drawio
│   ├── data_catalog.md
│   ├── data_flow.drawio
│   ├── data_models.drawio
│   ├── naming-conventions.md
│
├── scripts/                            # SQL scripts for ETL and transformations
│   ├── bronze/
│   ├── silver/
│   ├── gold/
│
├── tests/                              # Testing and data quality validation files
│
├── README.md
├── LICENSE
├── .gitignore
└── requirements.txt
```
## Portfolio Value

This project is well-suited for showcasing skills in:

- SQL Development
- Data Engineering
- ETL Pipeline Development
- Data Modeling
- Data Analytics

In addition to technical ability, it also demonstrates an end-to-end understanding of how raw data is transformed into meaningful business insights.

## License

This project is licensed under the MIT License, which allows the project to be used, modified, and shared with proper attribution.

---
# README Versi Indonesia
---
# SQL_Data_Warehouse_Project

Selamat datang di repository **Proyek Data Warehouse dan Analitik**.  
Proyek ini menampilkan implementasi **data warehouse modern** menggunakan **SQL Server**, mulai dari proses integrasi data hingga analisis untuk menghasilkan insight yang mendukung pengambilan keputusan bisnis. Proyek ini juga dirancang sebagai portofolio untuk menunjukkan penerapan praktik yang umum digunakan dalam **data engineering** dan **data analytics**.

---

## Gambaran Umum Proyek

Proyek ini berfokus pada pembangunan data warehouse yang mampu mengintegrasikan data dari berbagai sumber ke dalam satu sistem terpusat. Proses yang dibangun mencakup:

- Pengambilan data dari sistem sumber
- Pembersihan dan transformasi data
- Pemodelan data untuk kebutuhan analitis
- Pembuatan analisis dan laporan berbasis SQL

Hasil akhirnya adalah model data yang siap digunakan untuk kebutuhan pelaporan, dashboard, dan analisis bisnis.

---

## Arsitektur Data

Proyek ini menggunakan pendekatan **Medallion Architecture** yang terdiri dari tiga lapisan utama:

### Bronze Layer
Lapisan ini menyimpan data mentah dari sistem sumber dalam bentuk aslinya. Data diimpor dari file CSV ke dalam SQL Server tanpa banyak perubahan.

### Silver Layer
Lapisan ini digunakan untuk proses pembersihan, standarisasi, dan normalisasi data agar kualitas data menjadi lebih baik dan konsisten.

### Gold Layer
Lapisan ini berisi data yang telah diproses dan dimodelkan agar siap digunakan untuk pelaporan, dashboard, dan analisis bisnis.

---

## Cakupan Proyek

Ruang lingkup proyek ini meliputi:

1. **Perancangan Arsitektur Data**  
   Membangun data warehouse modern dengan struktur berlapis menggunakan pendekatan Bronze, Silver, dan Gold.

2. **Pipeline ETL**  
   Mengekstrak, mentransformasi, dan memuat data dari sistem sumber ke dalam data warehouse.

3. **Pemodelan Data**  
   Mengembangkan **fact table** dan **dimension table** yang dioptimalkan untuk kebutuhan query analitis.

4. **Analitik dan Pelaporan**  
   Membuat analisis serta laporan berbasis SQL untuk menghasilkan insight yang dapat digunakan oleh stakeholder.

---

## Tujuan Proyek

Tujuan utama proyek ini adalah membangun data warehouse modern menggunakan SQL Server untuk mengonsolidasikan data penjualan dari beberapa sumber agar dapat digunakan untuk analisis dan pelaporan secara lebih efektif.

Secara khusus, proyek ini bertujuan untuk:

- Mengimpor data dari dua sistem sumber, yaitu **ERP** dan **CRM**
- Membersihkan dan memperbaiki kualitas data sebelum analisis
- Menggabungkan data ke dalam model data yang terintegrasi dan mudah digunakan
- Menyediakan dokumentasi yang jelas untuk mendukung kebutuhan bisnis dan analitik

> Catatan: Proyek ini berfokus pada dataset terbaru dan tidak mencakup historisasi data.

---

## Fokus Analisis

Analisis dalam proyek ini difokuskan pada tiga area utama:

- **Perilaku Pelanggan**
- **Kinerja Produk**
- **Tren Penjualan**

Melalui analisis berbasis SQL, proyek ini bertujuan menghasilkan insight yang dapat membantu proses evaluasi bisnis dan pengambilan keputusan yang lebih tepat.

---

## Tools yang Digunakan

Beberapa tools yang digunakan dalam proyek ini antara lain:

- **SQL Server Express** — database engine untuk menyimpan dan mengelola data
- **SQL Server Management Studio (SSMS)** — tool untuk pengelolaan database dan eksekusi query
- **Draw.io** — untuk membuat diagram arsitektur, alur data, dan model data
- **GitHub** — untuk version control dan dokumentasi project

---

## Struktur Repository

```bash
data-warehouse-project/
│
├── datasets/                           # Dataset mentah dari sistem ERP dan CRM
│
├── docs/                               # Dokumentasi proyek dan arsitektur
│   ├── etl.drawio
│   ├── data_architecture.drawio
│   ├── data_catalog.md
│   ├── data_flow.drawio
│   ├── data_models.drawio
│   ├── naming-conventions.md
│
├── scripts/                            # Script SQL untuk ETL dan transformasi
│   ├── bronze/
│   ├── silver/
│   ├── gold/
│
├── tests/                              # File pengujian dan validasi kualitas data
│
├── README.md
├── LICENSE
├── .gitignore
└── requirements.txt
```
---
## Nilai Portofolio

Proyek ini dapat digunakan untuk menunjukkan kemampuan dalam bidang:

- SQL Development
- Data Engineering
- ETL Pipeline Development
- Data Modeling
- Data Analytics

Selain kemampuan teknis, proyek ini juga menunjukkan pemahaman menyeluruh terhadap alur data, mulai dari data mentah hingga menjadi insight yang siap digunakan.

---
## Lisensi

Project ini menggunakan lisensi MIT, sehingga dapat digunakan, dimodifikasi, dan dibagikan dengan tetap mencantumkan atribusi yang sesuai.
