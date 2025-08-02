# Peluang Kekeringan Berdasarkan Karakteristik Suhu Permukaan, Kehijauan Vegetasi, dan Presipitasi di Sub DAS Cikapundung

Penelitian ini bertujuan untuk menganalisis peluang kejadian kekeringan dengan pendekatan spasial dan statistik berdasarkan tiga parameter utama, yaitu suhu permukaan, keragaman vegetasi (NDVI), dan presipitasi. Studi kasus dilakukan pada wilayah Sub DAS Cikapundung, Bandung.

## 👤 Penulis

**Miftahul Ardli**  
NIM: 150510180225  
Program Studi Agroteknologi  
Fakultas Pertanian  
Universitas Padjadjaran

---

## 🧪 Deskripsi Proyek

Analisis dilakukan dengan pendekatan kuantitatif berbasis Python dan Google Earth Engine, menggunakan regresi linear dan Random Forest untuk memodelkan hubungan antara LST, NDVI, dan CHIRPS terhadap SPI-3. Eksplorasi data spasial-temporal dilakukan melalui visualisasi, korelasi, dan interpolasi spasial.

---

## 🛠 Environment & Tools

## ⚙️ Environment

Proyek ini dikembangkan menggunakan:

- **Python** ≥ 3.8
- **Jupyter Notebook** (via Anaconda atau VS Code)
- Ekstraksi data dilakukan di **Google Earth Engine** (GEE) menggunakan JavaScript API.

### 📦 Library Python yang Digunakan

- `numpy` – operasi numerik
- `pandas` – manipulasi dan analisis data tabular
- `matplotlib` & `seaborn` – visualisasi grafik & distribusi
- `scikit-learn` – model machine learning (Random Forest, KNN, Gradient Boosting)
- `statsmodels` – regresi linear & uji statistik
- `scipy` – interpolasi spasial (`griddata`) dan fungsi statistik
- `joblib` – menyimpan model (.pkl)


---

## 🔍 Metodologi

1. **Ekstraksi data LST, NDVI, dan CHIRPS** secara bulanan (2013–2022) menggunakan Google Earth Engine (GEE)
2. **Penghitungan nilai SPI-3** (Standardized Precipitation Index) dari data CHIRPS menggunakan distribusi Gamma
3. **Pembersihan dan penggabungan data** menjadi dataset spasial-temporal
4. **Analisis statistik deskriptif, korelasi Pearson, dan regresi linear multivariat**
5. **Pemodelan prediktif** menggunakan algoritma *Random Forest Regressor* (dibandingkan dengan KNN, Gradient Boosting, dan regresi linear)
6. **Visualisasi** hasil analisis dalam bentuk grafik time-series, scatterplot, learning curve, serta peta interpolatif berbasis `scipy.interpolate.griddata`

---

## 🌐 Sumber Data

Seluruh data dikumpulkan dari sumber terbuka melalui platform Google Earth Engine:

- **Land Surface Temperature (LST)** dan **NDVI**:  
  → *Landsat 8 Collection 1 Tier 1* – disediakan oleh **USGS & NASA**

- **Presipitasi**:  
  → *CHIRPS Daily v2.0* – dikembangkan oleh **Climate Hazards Center (CHC), UCSB, USGS**, dengan dukungan **USAID, NASA, NOAA**
---

## 🔒 Catatan

Karena keterbatasan lisensi  dan ukuran file, sebagian data mungkin tidak tersedia dalam repositori publik. Silakan hubungi penulis untuk akses lebih lanjut.

---

## 📜 Lisensi

Repositori ini dibuat untuk keperluan akademik (skripsi) dan tidak dimaksudkan untuk penggunaan komersial tanpa izin tertulis. Silakan cantumkan kutipan jika mengadaptasi sebagian kode atau analisis.

---

## 📫 Kontak

Jika ada pertanyaan atau kolaborasi, silakan hubungi:

**Miftahul Ardli**  
Email: mifardli21@gmail.com/ miftahul18002@unpad.ac.id
Linkedin: https://linkedin.com/in/mifardli

---
