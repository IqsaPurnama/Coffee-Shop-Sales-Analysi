# Project Machine Learning: Prediksi Kategori Produk Kedai Kopi

**Nama:** Iqsa Purnama Saputra
**NIM:** [241011400827]
**Program Studi:** Teknik Informatika, Universitas Pamulang
**Mata Kuliah:** Machine Learning

## Deskripsi
Project ini mengerjakan tahapan Machine Learning dari pengenalan sampai
Data Splitting menggunakan data transaksi penjualan kedai kopi.

## Dataset
- **Sumber:** Kaggle, "Coffee Shop Sales Analysis" oleh divu2001
  https://www.kaggle.com/datasets/divu2001/coffee-shop-sales-analysis
- **Isi:** 149.116 baris, 18 kolom, transaksi 3 toko, Januari-Juni 2023
- **Catatan:** sebagian kolom (Total_Bill, Size, Month Name, Day Name, Hour, Month, Day of Week) adalah kolom turunan pada file yang digunakan.

## Tahapan yang Dikerjakan
1. Data Collecting
2. Data Loading
3. Data Cleaning (cek tipe data, missing value, duplikat, outlier)
4. Data Transformation (penentuan fitur dan target, One-Hot Encoding)
5. EDA & ExDA (distribusi, korelasi, visualisasi)
6. Data Splitting (80:20, random_state=42, stratify)

## Fitur dan Target
- **Target (y):** product_category
- **Fitur (X):** store_location, transaction_qty, Size, Hour, Month, Day of Week

## Hasil Data Splitting
- Data latih: 119.292 baris
- Data uji: 29.824 baris

## Struktur Folder
- `project_ml.ipynb`: notebook pengerjaan
- `data/Project.csv`: dataset
- `requirements.txt`: daftar library

## Cara Menjalankan
```bash
conda create -n ml-project python=3.11 -y
conda activate ml-project
pip install -r requirements.txt
jupyter notebook
```
Lalu buka `project_ml.ipynb` dan jalankan semua cell (Kernel → Restart & Run All).
