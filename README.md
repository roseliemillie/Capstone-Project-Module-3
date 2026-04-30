# 📊 Bank Marketing Campaign Prediction

## 📌 Project Introduction
Project ini bertujuan untuk membantu bank dalam meningkatkan efektivitas campaign marketing produk **term deposit** dengan memanfaatkan Machine Learning.

Pada kondisi saat ini, campaign dilakukan secara massal tanpa prioritas yang jelas, sehingga banyak sumber daya terbuang untuk menghubungi nasabah yang tidak potensial. Berdasarkan data historis, hanya sekitar **47.8% nasabah yang berhasil subscribe**, sementara lebih dari **52% tidak memberikan hasil**.

Dengan membangun model prediktif, project ini berfokus untuk:
- Mengidentifikasi nasabah dengan probabilitas tinggi untuk subscribe
- Mengurangi biaya operasional campaign
- Meningkatkan conversion rate
- Membantu pengambilan keputusan berbasis data

Model yang dibangun menggunakan pendekatan **Machine Learning Classification** untuk memprediksi apakah nasabah akan subscribe (yes/no).

## 🎯 Business Problem
Tanpa sistem prediksi:
- Agen menghubungi semua nasabah secara acak
- Banyak waktu dan biaya terbuang
- Prospek potensial bisa terlewat

Dengan model:
- Nasabah dapat diprioritaskan berdasarkan peluang subscribe
- Campaign menjadi lebih efisien dan terarah

## 🎯 Objective
Membangun model Machine Learning untuk:
- Memprediksi kemungkinan nasabah subscribe term deposit
- Memberikan **probability score** untuk membantu prioritas campaign
- Meningkatkan efisiensi dan efektivitas marketing

## 📊 Dataset Overview
Dataset berisi:
- **7,805 data nasabah**
- **10 fitur input**
- Target: `deposit` (yes/no)

### Feature Categories:
- Demografi: age, job
- Finansial: balance, housing, loan
- Campaign: contact, month, campaign
- Histori: pdays, poutcome

## ⚙️ Machine Learning Approach

### Model:
- Gradient Boosting Classifier (Final Model)

### Kenapa dipilih?
Model ini memiliki performa terbaik berdasarkan hasil cross-validation.

### Evaluation Metrics:
- **F1-Score (Primary)** → balance antara precision & recall
- ROC-AUC (Secondary)

Alasan:
- False Negative → kehilangan customer potensial
- False Positive → pemborosan resource

## 📈 Key Insights
Beberapa insight penting dari analisis:
- Channel **cellular** memiliki conversion rate lebih tinggi
- Nasabah dengan **poutcome = success** memiliki peluang subscribe tertinggi (~91%) :contentReference[oaicite:0]{index=0}
- Bulan seperti **March, December, October, September** memiliki conversion rate lebih tinggi :contentReference[oaicite:1]{index=1}
- Campaign terlalu sering dapat menurunkan peluang subscribe

## 📉 Business Impact

### Sebelum ML:
- Campaign dilakukan tanpa prioritas
- Biaya tinggi
- Conversion rendah

### Setelah ML:
- Prioritas berdasarkan probability score
- Efisiensi waktu agen meningkat
- Lebih sedikit prospek potensial terlewat

Menurut hasil evaluasi:
- Recall meningkat hingga ~74.66% :contentReference[oaicite:2]{index=2}
- Model lebih efektif dalam menangkap calon subscriber

## 📌 Conclusion
Model Machine Learning berhasil membantu:
- Mengidentifikasi nasabah potensial
- Meningkatkan efisiensi campaign
- Mendukung pengambilan keputusan berbasis data

## 💡 Recommendation
- Gunakan model untuk prioritas campaign (bukan menggantikan keputusan bisnis)
- Fokus pada nasabah dengan probability tinggi
- Pertimbangkan faktor:
  - Channel komunikasi
  - Waktu campaign
  - Riwayat interaksi

### Improvement:
- Tambah fitur seperti:
  - Durasi call
  - Biaya campaign
  - Estimasi revenue
- Gunakan explainability (SHAP)

## 👩‍💻 Author
Millitia Christy Eirene Roselie  
Data Science & Machine Learning Project
