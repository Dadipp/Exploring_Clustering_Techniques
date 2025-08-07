# 🧠 Customer Segmentation using K-Means Clustering

## 📌 Project Overview

Proyek ini bertujuan untuk melakukan **segmentasi pelanggan** menggunakan algoritma **K-Means Clustering** pada dataset pelanggan dari sebuah pusat perbelanjaan. Tujuan utamanya adalah mengelompokkan pelanggan berdasarkan pola pembelian mereka untuk mendukung strategi pemasaran yang lebih tepat sasaran.

## 📊 Dataset

Dataset yang digunakan merupakan data pelanggan dengan fitur berikut:

- **CustomerID**: ID pelanggan
- **Gender**: Jenis kelamin pelanggan
- **Age**: Usia pelanggan
- **Annual Income (k$)**: Pendapatan tahunan pelanggan dalam ribuan dolar
- **Spending Score (1-100)**: Skor pengeluaran yang menunjukkan perilaku belanja pelanggan

## 🧪 Metodologi

1. **Exploratory Data Analysis (EDA)**:
   - Visualisasi distribusi umur, penghasilan, dan spending score
   - Scatter plot untuk melihat hubungan antara income dan spending score
   - Boxplot untuk membandingkan pengeluaran berdasarkan gender

2. **Data Preprocessing**:
   - Pemilihan fitur: `['Age', 'Annual Income (k$)', 'Spending Score (1-100)']`
   - Standardisasi fitur menggunakan `StandardScaler`

3. **Menentukan Jumlah Cluster**:
   - **Metode Elbow**: Digunakan untuk memilih jumlah cluster optimal berdasarkan nilai inertia
   - **Silhouette Score**: Digunakan sebagai validasi kualitas cluster

4. **Clustering dengan K-Means**:
   - Implementasi model K-Means
   - Visualisasi hasil clustering dalam bentuk scatter plot 2D dan 3D

5. **Interpretasi Segmentasi**:
   - Analisis karakteristik tiap cluster berdasarkan usia, penghasilan, dan spending score

## 🔧 Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (`KMeans`, `StandardScaler`, `silhouette_score`)

## 📈 Visualizations

- Histogram distribusi fitur
- Heatmap korelasi antar variabel
- Scatter plot hasil clusterisasi
- Elbow plot dan Silhouette Score plot

## 💡 Insights

- Terdapat **5 segmen pelanggan** yang dapat dibedakan berdasarkan tingkat pendapatan dan skor pengeluaran.
- Salah satu segmen menunjukkan pelanggan dengan **pendapatan tinggi tetapi pengeluaran rendah**, yang potensial untuk ditingkatkan engagement-nya.
- Segmen lain terdiri dari pelanggan dengan **pengeluaran tinggi namun pendapatan sedang**, yang kemungkinan besar merupakan target ideal untuk strategi promosi.
- Visualisasi 3D membantu dalam memahami distribusi cluster secara menyeluruh.
