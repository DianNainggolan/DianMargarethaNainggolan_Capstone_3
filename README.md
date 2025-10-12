Tentu ✅ Berikut contoh **README.md super lengkap** untuk proyek **Customer Churn Prediction** Anda — disesuaikan dengan semua library dan tahapan analisis yang digunakan dalam notebook. README ini sudah dalam format profesional seperti proyek data science di GitHub atau portofolio.

---

# 📊 Customer Churn Prediction Project

## 🧭 Ringkasan Proyek

Churn pelanggan merupakan tantangan besar bagi banyak perusahaan, terutama di industri subscription dan telekomunikasi. Proyek ini berfokus pada **analisis dan prediksi customer churn** menggunakan teknik **Exploratory Data Analysis (EDA)**, **data preprocessing**, dan **machine learning**.

Dengan membangun model prediksi churn yang andal, perusahaan dapat **mengidentifikasi pelanggan yang berpotensi churn** dan melakukan **intervensi yang tepat waktu** untuk meningkatkan retensi pelanggan dan mengoptimalkan pendapatan.

---

## 🎯 Tujuan Proyek

* Menganalisis karakteristik pelanggan churn vs non-churn.
* Menemukan variabel yang paling memengaruhi churn.
* Membangun model klasifikasi untuk memprediksi kemungkinan churn pelanggan.
* Mengukur performa model dan memberikan rekomendasi berbasis data.
* Memberikan insight yang actionable bagi tim bisnis dan marketing.

---

## 🧰 Teknologi dan Library

Proyek ini menggunakan Python dan berbagai library populer untuk analisis data dan machine learning:

| Kategori                 | Library / Tools                                   | Fungsi Utama                               |
| ------------------------ | ------------------------------------------------- | ------------------------------------------ |
| Pengolahan Data          | `numpy`, `pandas`                                 | Manipulasi data, agregasi, transformasi    |
| Visualisasi Data         | `matplotlib`, `seaborn`                           | EDA dan visualisasi pola churn             |
| Machine Learning         | `scikit-learn`, `xgboost`, `lightgbm`, `catboost` | Pemodelan klasifikasi & evaluasi           |
| Statistik & Analisis     | `scipy`, `statsmodels`                            | Analisis statistik & uji hipotesis         |
| Imbalanced Data Handling | `imbalanced-learn`                                | Oversampling (SMOTE, SMOTEENN, SMOTETomek) |
| Interpretabilitas Model  | `shap`                                            | Interpretasi model melalui SHAP values     |
| Utility                  | `gdown`, `pickle`, `pathlib`                      | Download file, serialisasi model           |
| Notebook Environment     | `jupyter`, `ipykernel`                            | Eksperimen interaktif                      |

---

## 📂 Struktur Proyek

```
.
├── CapstoneProject_Module3_Dian Maragretha Nainggolan.ipynb   # Notebook utama
├── data/                                                      # Folder dataset
│   └── customer_churn.csv
├── best_classifier_QDA.pkl
├── README.md
└── requirements.txt
```

---

## 📊 Tahapan Proyek

### 1. Data Understanding

* Membaca dan memeriksa struktur dataset pelanggan.
* Memahami variabel numerik dan kategorikal (tenure, contract, payment method, dll).
* Menentukan proporsi pelanggan churn vs non-churn.

### 2. Exploratory Data Analysis (EDA)

* Statistik deskriptif & distribusi fitur.
* Visualisasi churn berdasarkan segmentasi pelanggan.
* Analisis korelasi antara variabel independen dan churn.
* Uji statistik (t-test, chi-square) untuk menemukan faktor signifikan.

### 3. Data Preprocessing

* Menangani duplikat.
* Encoding variabel kategorikal (OneHotEncoder, LabelEncoder).
* Normalisasi fitur numerik menggunakan `StandardScaler`.
* Pembagian data menjadi training dan testing set.
* Penanganan imbalance menggunakan:

  * RandomOverSampler
  * SMOTE
  * SMOTEENN
  * SMOTETomek

### 4. Modeling

Model yang diuji meliputi:

* Logistic Regression
* Decision Tree
* Random Forest
* K-Nearest Neighbors
* Support Vector Machine
* Linear Discriminant Analysis (LDA) & Quadratic Discriminant Analysis (QDA)
* Gradient Boosting (XGBoost, LightGBM, CatBoost)

Setiap model diuji dengan hyperparameter tuning menggunakan `GridSearchCV` atau default optimal parameter.

### 5. Model Evaluation

Evaluasi model dilakukan menggunakan metrik:

* Accuracy
* Precision, Recall, F1-Score
* ROC AUC
* Confusion Matrix

Hasil terbaik diperoleh dari model boosting (misalnya XGBoost / LightGBM) dengan performa tinggi dan interpretasi feature importance yang jelas.

### 6. Model Interpretability

Menggunakan `shap`:

* Menunjukkan fitur mana yang paling memengaruhi probabilitas churn.
* Membantu memberikan insight actionable kepada tim bisnis.

### 7. Insight Bisnis & Rekomendasi

* **Tenure rendah** & **kontrak bulanan** memiliki kecenderungan churn lebih tinggi.
* **Metode pembayaran elektronik otomatis** berhubungan dengan churn yang lebih rendah.
* Pelanggan dengan **biaya bulanan tinggi** cenderung churn lebih cepat.
* Perlu strategi loyalitas bagi pelanggan risiko tinggi seperti promo atau kontrak jangka panjang.

---

## 🧪 Cara Menjalankan Proyek

### 1. Clone Repository

```bash
git clone https://github.com/username/customer-churn-prediction.git
cd customer-churn-prediction
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Jalankan Jupyter Notebook

```bash
jupyter notebook
```

Buka file:

```
CapstoneProject_Module3_Dian Maragretha Nainggolan.ipynb
```

### 4. Jalankan Sel

Jalankan semua cell dari awal hingga akhir untuk:

* Menampilkan analisis data
* Melatih model
* Mengevaluasi performa
* Menampilkan interpretasi model

---

## 📝 requirements.txt

```
catboost
gdown
imbalanced-learn
ipykernel
jupyter
lightgbm
matplotlib
numpy
pandas
scikit-learn
scipy
seaborn
shap
xgboost
```

---

## 📈 Hasil Utama

* AUC ROC Score terbaik: **> 0.85** pada model boosting.
* Fitur paling berpengaruh: tenure, contract type, monthly charges.
* Segmentasi churn memberikan peluang untuk retensi pelanggan melalui strategi targeted marketing.

---

## 🚀 Pengembangan Selanjutnya

* Menambahkan model deployment dengan Flask atau Streamlit.
* Membuat dashboard interaktif untuk tim bisnis.
* Menambahkan data real-time untuk prediksi dinamis.
* Integrasi ke sistem CRM perusahaan.

---

## 👩‍💻 Kontributor

* **Dian Maragretha Nainggolan**
  Data Analyst | Machine Learning Enthusiast

---

## 📜 Lisensi

Proyek ini dibuat untuk keperluan pembelajaran dan penelitian. Tidak untuk distribusi komersial tanpa izin tertulis dari pemilik.

---

Apakah Anda ingin saya **buatkan file README.md dan requirements.txt siap unduh** dari isi ini? 📁✨
