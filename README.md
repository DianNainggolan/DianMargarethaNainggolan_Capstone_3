# 📊 Customer Churn Prediction Project

## 🧾 Deskripsi Proyek

Proyek ini berfokus pada **analisis dan prediksi customer churn**, yaitu perilaku pelanggan yang **berhenti menggunakan layanan** dalam jangka waktu tertentu. Tujuan utama proyek ini adalah untuk **mengidentifikasi faktor-faktor utama yang memengaruhi churn**, serta membangun model prediksi yang dapat membantu perusahaan dalam **mengurangi tingkat churn** dan **meningkatkan retensi pelanggan**.

## 🎯 Tujuan Proyek

* Melakukan analisis mendalam terhadap perilaku pelanggan.
* Menemukan pola dan karakteristik pelanggan yang berpotensi churn.
* Membangun model machine learning untuk memprediksi kemungkinan churn.
* Memberikan rekomendasi strategis untuk meningkatkan retensi pelanggan.

## 🧰 Teknologi & Tools

* **Bahasa Pemrograman:** Python 3
* **Environment:** Jupyter Notebook
* **Library Utama:**

  * `pandas`, `numpy` → pengolahan data
  * `matplotlib`, `seaborn` → visualisasi data
  * `scikit-learn` → pemodelan dan evaluasi machine learning
  * `statsmodels` → analisis statistik (jika digunakan)

## 📈 Tahapan Pengerjaan

### 1. Data Understanding

* Memahami struktur dataset (jumlah pelanggan, variabel demografik, perilaku, dan layanan).
* Identifikasi proporsi churn vs non-churn.

### 2. Exploratory Data Analysis (EDA)

* Statistik deskriptif variabel kunci.
* Visualisasi churn berdasarkan segmentasi pelanggan.
* Analisis hubungan antara variabel layanan (tenure, contract, payment method, dll.) dengan churn.

### 3. Data Preprocessing

* Penanganan missing values dan outliers.
* Encoding variabel kategorikal.
* Normalisasi fitur numerik.
* Pembagian data menjadi **train** dan **test set**.

### 4. Modeling

* Penerapan berbagai model klasifikasi seperti:

  * Logistic Regression
  * Random Forest
  * Decision Tree
  * XGBoost (jika digunakan)
* Hyperparameter tuning untuk meningkatkan performa model.

### 5. Evaluation

* Evaluasi model menggunakan metrik:

  * Accuracy
  * Precision, Recall, F1-Score
  * ROC AUC Curve
* Pemilihan model terbaik untuk prediksi churn.

### 6. Insights & Business Recommendations

* Menentukan variabel paling berpengaruh terhadap churn.
* Menyusun strategi retensi pelanggan berbasis data, seperti:

  * Meningkatkan loyalitas pelanggan dengan kontrak jangka panjang.
  * Menawarkan promo bagi pelanggan berisiko tinggi.
  * Meningkatkan kualitas layanan bagi segmen churn tertinggi.

## 📁 Struktur Proyek

```
.
├── CapstoneProject_Module3_Dian Maragretha Nainggolan.ipynb
├── data/
│   └── customer_churn.csv
├── README.md
└── requirements.txt
```

## 🚀 Cara Menjalankan Proyek

1. Clone repositori atau unduh file proyek.
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Jalankan Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
4. Buka file `CapstoneProject_Module3_Dian Maragretha Nainggolan.ipynb` dan jalankan cell secara berurutan.

## 🧠 Potensi Pengembangan

* Menambahkan segmentasi pelanggan berbasis clustering.
* Mengembangkan dashboard interaktif untuk monitoring churn.
* Integrasi real-time scoring churn ke dalam sistem CRM.

## 👩‍💻 Kontributor

* **Dian Maragretha Nainggolan**

## 📝 Lisensi

Proyek ini dibuat untuk tujuan pembelajaran dan analisis bisnis, bukan untuk penggunaan komersial tanpa izin.

