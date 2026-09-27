# Prediksi Gaji Karyawan (Employee Salary Prediction)

Proyek Machine Learning ini bertujuan untuk memprediksi **gaji (salary)** seorang karyawan berdasarkan variabel usia, gender, tingkat pendidikan, pengalaman kerja, dan jabatan (*Job Title*).

Proyek ini dibangun sebagai eksperimen untuk menangani fitur kategori berkardinalitas tinggi, menentukan teknik *encoding* yang tepat (ordinal vs nominal), serta membandingkan dan mengevaluasi model regresi.

---

## 🛠️ Alur Kerja Proyek

1. **Exploratory Data Analysis (EDA) & Data Cleaning**:
   - Memuat dataset `Salary Data.csv`.
   - Mengatasi nilai yang hilang (*missing values*) dan membuang baris anomali/outlier (`Salary = 350`).
   - Dataset akhir yang siap digunakan terdiri dari **372 baris data**.
   - Menganalisis distribusi target (`Salary`) serta fitur kategorikal (`Education Level`, `Job Title`).

2. **Pembersihan Outlier & Evaluasi Distribusi**:
   - Menguji *skewness* pada variabel target. Nilai *skewness* berada di angka `~0.4` (di bawah ambang batas 0.5), sehingga transformasi logaritma **tidak diperlukan**.

3. **Visualisasi Data**:
   - Membuat *scatter plot* dan grafik korelasi untuk menganalisis hubungan antara fitur numerik (`Age` dan `Years of Experience`) terhadap `Salary`.

4. **Data Preprocessing & Feature Engineering**:
   - *Encoding* variabel kategorikal dengan teknik yang sesuai (*One-Hot Encoding* / *Ordinal Encoding*).
   - Pemisahan data menjadi *training set* dan *testing set* (`train_test_split`).

5. **Pemodelan & Evaluasi**:
   - Melatih model regresi (seperti `RandomForestRegressor`).
   - Evaluasi performa model menggunakan metrik regresi standar (MAE, MSE, RMSE, R² Score).

---

## 🧰 Pustaka & Teknologi

* **Bahasa Pemrograman**: Python 3.x
* **Manipulasi & Analisis Data**: `pandas`, `numpy`
* **Visualisasi Data**: `matplotlib`, `seaborn`
* **Machine Learning**: `scikit-learn`
* **Statistik**: `scipy`
