# 🏥 Diabetes Health Indicators Prediction
A diabetes risk prediction system utilizing the **Random Forest Classifier** optimized with **SMOTE (Synthetic Minority Over-sampling Technique)**. This project analyzes lifestyle health indicators to classify individuals into three categories: Healthy, Prediabetes, or Diabetes.

*This project implements Machine Learning in the healthcare sector (Health-Tech) to support early detection of chronic diseases through public health indicator data.*

## 📝 Project Description
Using CDC health indicator datasets, this project aims to map the relationship between lifestyle factors (such as BMI, physical activity, and smoking) and diabetes risk. The primary challenge in this medical dataset is the highly imbalanced class distribution, addressed through oversampling techniques to ensure the model accurately detects Diabetes and Prediabetes cases.

## ✨ Key Features
- **Multi-class Classification**: Predicts three distinct health statuses (Healthy, Prediabetes, Diabetes).
- **SMOTE Balancing**: Employs data synthesis to handle minority class imbalances (specifically Prediabetes).
- **Feature Importance Analysis**: Identifies top risk factors (e.g., high blood pressure and cholesterol) that most significantly influence diabetes status.
- **Automated Diagnostic Function**: Features a `predict_diabetes_risk` function for instantaneous new patient data processing.

## 🛠️ Tech Stack & Implementation
- **Machine Learning**: Scikit-Learn (Random Forest, Logistic Regression).
- **Imbalanced Learning**: Imbalanced-learn (SMOTE).
- **Data Manipulation**: Pandas & NumPy.
- **Visualization**: Matplotlib & Seaborn (for medical feature correlation analysis).
- **Environment**: Google Colab & Kaggle API.

## 📊 Methodology
- **Data Exploration**: Analyzing demographic and lifestyle feature distributions relative to diabetes status.
- **Handling Imbalance**: Applying SMOTE to training data to establish balance between target classes, preventing model bias.
- **Model Training**: Utilizing Random Forest to manage non-linear patterns in complex health data.
- **Clinical Validation**: Evaluating performance via Confusion Matrices to minimize False Negatives in medical diagnoses.

## ⚙️ Installation & Usage

### 1. Prerequisites (Kaggle API)

This project uses the CDC Diabetes Health Indicators dataset from Kaggle.

  - Place your `kaggle.json` in the appropriate directory (`~/.kaggle/` or Colab Secrets).
  - The notebook will handle the download of the [Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset).

### 2. Environment Setup

```bash
# Clone the repository
git clone https://github.com/Billy1205/diabetes-prediction.git
cd diabetes-prediction

# Install health-tech stack
pip install -r requirements.txt
```

### 3. Execution

1.  Open `notebooks/diabetes-prediction.ipynb`.
2.  Run all cells to perform **SMOTE oversampling** and train the **Random Forest** model.
3.  Use the built-in function `predict_diabetes_risk` to test the model with custom patient data.

***

# 🏥 Diabetes Health Indicators Prediction
Sistem prediksi risiko diabetes menggunakan algoritma **Random Forest Classifier** yang dioptimalkan dengan teknik **SMOTE (Synthetic Minority Over-sampling Technique)**. Proyek ini menganalisis indikator kesehatan gaya hidup untuk mengklasifikasikan individu ke dalam tiga kategori: Sehat, Prediabetes, atau Diabetes.

*Proyek ini merupakan implementasi Machine Learning dalam bidang kesehatan (Health-Tech) untuk mendukung deteksi dini penyakit kronis melalui data indikator kesehatan masyarakat.*

## 📝 Project Description
Menggunakan dataset indikator kesehatan dari CDC (Centers for Disease Control and Prevention), proyek ini bertujuan untuk memetakan hubungan antara gaya hidup (seperti BMI, aktivitas fisik, merokok) dengan risiko diabetes. Tantangan utama dalam data medis ini adalah distribusi kelas yang sangat tidak seimbang, yang diatasi dengan teknik *oversampling* untuk memastikan model mampu mendeteksi kasus Diabetes dan Prediabetes dengan akurasi yang lebih baik.

## ✨ Key Features
- **Multi-class Classification**: Memprediksi tiga status kesehatan sekaligus (Healthy, Prediabetes, Diabetes).
- **SMOTE Balancing**: Menggunakan teknik sintesis data untuk mengatasi ketidakseimbangan kelas minoritas (Prediabetes).
- **Feature Importance Analysis**: Mengidentifikasi faktor risiko utama (seperti tekanan darah tinggi dan kolesterol) yang paling berpengaruh terhadap diabetes.
- **Automated Diagnostic Function**: Menyediakan fungsi `predict_diabetes_risk` yang dapat memproses data pasien baru secara instan.
- **Robust Preprocessing**: Integrasi penanganan nilai hilang, duplikat, dan standarisasi fitur medis.

## 📊 Methodology
- **Data Exploration**: Analisis distribusi fitur demografis dan gaya hidup terhadap status diabetes.
- **Handling Imbalance**: Menerapkan SMOTE pada data training untuk menciptakan keseimbangan antar kelas target agar model tidak bias.
- **Model Training**: Pelatihan model menggunakan Random Forest untuk menangani pola non-linear pada data kesehatan yang kompleks.
- **Clinical Validation**: Evaluasi menggunakan Confusion Matrix untuk meminimalkan *False Negatives* pada diagnosa medis.

## ⚙️ Instalasi & Penggunaan

### 1. Prasyarat (Kaggle API)

  - Pastikan kredensial Kaggle (`kaggle.json`) sudah siap untuk mengunduh dataset CDC secara otomatis.
  - Proyek ini akan memakai dataset [Diabetes Health Indicators Dataset](https://www.kaggle.com/datasets/alexteboul/diabetes-health-indicators-dataset).

### 2. Persiapan Lingkungan

```bash
# Klon repositori
git clone https://github.com/Billy1205/diabetes-prediction.git
cd diabetes-prediction

# Instal dependensi
pip install -r requirements.txt
```

### 3. Menjalankan Prediksi

1.  Buka notebook di folder `notebooks/`.
2.  Jalankan semua sel untuk melakukan pemrosesan **SMOTE** dan melatih model.
3.  Anda bisa mencoba fungsi `predict_diabetes_risk` untuk memasukkan data kesehatan baru dan melihat hasilnya secara instan.
