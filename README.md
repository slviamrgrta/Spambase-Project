# 📧 Spam Email Classification with Machine Learning

## 📁 Project Description
Proyek ini bertujuan untuk mengklasifikasikan email sebagai **spam** atau **non-spam** dengan memanfaatkan algoritma Machine Learning, khususnya **XGBoost**. Proyek ini dikembangkan sebagai bagian dari Ujian Akhir Semester mata kuliah *Machine Learning* di Universitas Bunda Mulia.

Dataset yang digunakan memiliki 4601 baris dan 58 kolom, mencakup berbagai atribut numerik yang merepresentasikan frekuensi kata, karakter, dan huruf kapital dalam isi email.

---

## 🧠 Methodology
Langkah-langkah yang dilakukan dalam proyek ini:
1. **Exploratory Data Analysis (EDA)**  
   - Analisis distribusi data dan deteksi outlier
2. **Feature Engineering**  
   - Penanganan nilai hilang dengan KNNImputer  
   - Penanganan outlier menggunakan metode IQR
3. **Data Preprocessing**  
   - Feature scaling menggunakan `StandardScaler`  
   - Pembagian data (80% train, 20% test)
4. **Imbalanced Data Handling**  
   - Menggunakan SMOTE untuk menyeimbangkan jumlah kelas spam dan non-spam
5. **Modeling**  
   - Algoritma: XGBoost  
   - Perbandingan kinerja model pada data imbalance vs balanced
6. **Evaluation**  
   - Confusion matrix  
   - Evaluasi metrik klasifikasi

---

## 📊 Tools & Technologies
- Python
- scikit-learn
- XGBoost
- imbalanced-learn (SMOTE)
- pandas, numpy
- matplotlib, seaborn

---

## ✅ Results
Confusion matrix hasil prediksi:
- **True Negative (non-spam benar):** 511  
- **False Positive (non-spam salah jadi spam):** 20  
- **False Negative (spam salah jadi non-spam):** 54  
- **True Positive (spam benar):** 336

Model terbaik diperoleh dengan menggunakan **XGBoost** pada data imbalance, tanpa SMOTE, untuk menjaga distribusi data asli.


