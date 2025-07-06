# Customer Churn Prediction & Executive Dashboard

## Deskripsi Proyek

Proyek ini merupakan kombinasi antara **Data Analysis** dan **Machine Learning**, dengan tujuan untuk memprediksi pelanggan yang berpotensi berhenti (*churn*) dari layanan perusahaan berbasis data historis. Proyek ini dilengkapi dengan visualisasi dashboard di **Looker Studio** agar mudah dipahami oleh stakeholder non-teknis.

---

## Tujuan Bisnis

- Mengidentifikasi pelanggan yang berisiko churn.
- Memberikan insight tentang faktor-faktor penyebab churn (jenis kontrak, layanan internet, biaya bulanan).
- Menyediakan visualisasi data yang mendukung pengambilan keputusan tim manajemen.

---

## Tools & Teknologi

- **Google Colab** – untuk pengolahan data & training model
- **Scikit-learn** – untuk pemodelan Machine Learning
- **Google Sheets** – sebagai jembatan data ke dashboard
- **Looker Studio** – untuk visualisasi hasil akhir
- **Pandas, Numpy, Seaborn** – untuk analisis data

---

## Alur Proyek

### 1. Data Understanding
Dataset: `Telco Customer Churn` dari Kaggle  
Isi data: kontrak pelanggan, jenis layanan, pembayaran, status churn, dll.

### 2. Data Preparation
- Mengubah tipe data `TotalCharges` ke numerik
- Menghapus data kosong dan kolom ID
- Encoding semua fitur kategorikal

### 3. Model Building
- Menggunakan **Logistic Regression**
- Train-test split (80-20)
- Evaluasi model dengan classification report & confusion matrix

### 4. Output & Export
- Hasil prediksi (`Predicted_Churn`) digabung dengan data aktual (`Actual_Churn`)
- Disimpan dalam file CSV untuk kebutuhan dashboard

### 5. Dashboard
- Menggunakan Google Looker Studio
- Visual utama:
  - Pie Chart Churn vs Tidak
  - Bar Chart berdasarkan Kontrak dan Layanan Internet
  - Rata-rata biaya bulanan berdasarkan status churn
  - Filter interaktif: gender, metode pembayaran, kontrak

---

## Hasil & Insight

- Pelanggan kontrak bulanan cenderung lebih banyak churn
- Biaya bulanan yang tinggi berkorelasi dengan churn
- Pelanggan dengan layanan **Fiber Optic** lebih sering churn dibanding DSL atau tanpa internet

---

## Kelebihan Proyek

- Menggabungkan analisis data dan prediksi berbasis ML
- Menyajikan insight dalam bentuk dashboard yang komunikatif
- Studi kasus churn sangat relevan di industri
- Dibuat dengan tools gratis dan mudah diakses

---

## Keterbatasan

- Model ML masih dasar (Logistic Regression)
- Belum ada hyperparameter tuning atau validasi silang
- Belum dilakukan deployment model ke API/web
- Dashboard bersifat statis (belum segmentasi otomatis atau rekomendasi retensi)

---
Jika tertarik berdiskusi atau berkolaborasi:  
**Gerry Aria Rotama**  
📧 Geerxv@gmail.com  
🌐 https://www.linkedin.com/in/geriariarotama/

