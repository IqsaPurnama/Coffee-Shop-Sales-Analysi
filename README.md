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
7. Modeling (Logistic Regression, Decision Tree, Random Forest)
8. Deployment & Monitoring (simpan model, simulasi prediksi, logging)

## Fitur dan Target
- **Target (y):** product_category
- **Fitur (X):** store_location, transaction_qty, Size, Hour, Month, Day of Week

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

## Referensi
1. Gooljar, S., Manohar, K., & Hosein, P. (2023). Performance Evaluation and Comparison of a New Regression Algorithm. *Proceedings of the 12th International Conference on Data Science, Technology and Applications (DATA)*, 524–531. https://www.scitepress.org/Documents/2023/121354

2. Aljuboori, A., & Abdulrazzq, M. M. A. (2024). Enhancing Accuracy in Predicting Continuous Values through Regression. *Iraqi Journal for Computer Science and Mathematics*, 5(4), Article 25. https://doi.org/10.52866/2788-7421.1227

3. Preuss, E., Argenta, Í. P., Franciscatto, R., & Pertile, S. de L. (2026). Análise comparativa de algoritmos de predição em dados tabulares: regressão linear, Random Forest, Gradient Boosting e redes neurais MLP. *RECIMA21*, 7, e768276. https://doi.org/10.47820/recima21.v7i7.8276
