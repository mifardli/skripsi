#  Drought Probability Based on Land Surface Temperature, Vegetation Greenness, and Precipitation in the Cikapundung Sub-Watershed

![Repo Views](https://komarev.com/ghpvc/?username=mifardli&repo=skripsi&color=blue)

Recorded from: Sat, 27 December 2025.

This research aims to analyze drought probability using spatial and statistical approaches based on three key parameters: land surface temperature (LST), vegetation greenness (NDVI), and precipitation. The case study is focused on the Cikapundung Sub-watershed area specific Lembang, Indonesia.

## 👤 Author

**Miftahul Ardli**  
Student ID: 150510180225  
Agrotechnology Study Program  
Department of Soil Science and Land Resources  
Faculty of Agriculture  
Universitas Padjadjaran

---

## 🧪 Project Description

The analysis was conducted using a quantitative approach based on Python and Google Earth Engine. Regression (linear and Random Forest) models were used to examine the relationship between LST, NDVI, and CHIRPS toward SPI-3 drought index. Spatio-temporal data exploration was performed through correlation analysis, interpolation, and data visualization.

---

## ⚙️ Environment & Tools

This project was developed using:

- **Python** ≥ 3.8  
- **Jupyter Notebook** (via Anaconda or VS Code)  
- Data extraction was performed via **Google Earth Engine** (JavaScript API)

### 📦 Python Libraries

- `numpy` – numerical operations  
- `pandas` – data manipulation and analysis  
- `matplotlib`, `seaborn` – data visualization  
- `scikit-learn` – machine learning (Random Forest, KNN, Gradient Boosting)  
- `statsmodels` – linear regression & statistical testing  
- `scipy` – spatial interpolation (`griddata`) and stats functions  
- `joblib` – saving model artifacts (.pkl)

---

## 🔍 Methodology

1. **Data extraction of LST, NDVI, and CHIRPS** on a monthly scale (2013–2022) using Google Earth Engine (GEE)  
2. **SPI-3 computation** (Standardized Precipitation Index) from CHIRPS using Gamma distribution  
3. **Cleaning and merging datasets** into a composite spatio-temporal format  
4. **Statistical analysis** (descriptive statistics, Pearson correlation, multivariate linear regression)  
5. **Predictive modeling** using Random Forest Regressor (compared with KNN, Gradient Boosting, Linear Regression)  
6. **Visualization**: time-series plots, scatterplots, learning curves, and spatial interpolation using `scipy.interpolate.griddata`

---

## 🌐 Data Sources

All datasets were retrieved from open sources via Google Earth Engine:

- **LST & NDVI**:  
  → *Landsat 8 Collection 1 Tier 1* – provided by **USGS & NASA**

- **Precipitation**:  
  → *CHIRPS Daily v2.0* – developed by **Climate Hazards Center (CHC), UCSB, USGS**  
  with support from **USAID, NASA, and NOAA**

---

## 🔒 Note

Due to licensing and size limitations, some data may not be publicly included in this repository. Please contact the author for access or inquiries.

---

## 📜 License

This repository is for academic and research purposes only (undergraduate thesis). Please provide proper citation if using or adapting parts of the analysis or code. Commercial use is not permitted without written permission.

---

## 📫 Contact

**Miftahul Ardli**  
Email: mifardli21@gmail.com / miftahul18002@unpad.ac.id  
LinkedIn: [linkedin.com/in/mifardli](https://linkedin.com/in/mifardli)

---
## ⚡ Bonus: XGBoost Model

In addition to the main Random Forest model, this project also includes an experimental implementation of the **XGBoost** algorithm (*Extreme Gradient Boosting*) to compare performance in drought prediction.

XGBoost is known for its speed and accuracy in regression tasks and is widely used in data science competitions and real-world applications. Although the Random Forest model performed best in this study, the inclusion of XGBoost provides an additional benchmark and enhances model comparison.

---

## 🙏 Acknowledgements

This project is part of the undergraduate thesis submitted to obtain a Bachelor’s degree in Agriculture at Universitas Padjadjaran. I would like to express my deepest gratitude to the individuals who provided academic guidance and feedback throughout this work:

- **Prof. Dr. Ir. H. Mahfud Arifin, MS** – Chief Thesis Advisor  
- **Dr. Muhammad Amir Solihin, SP, MT** – Co-Advisor & Head of Study Program  
- **Ade Setiawan, SP, MP** – Primary Reviewer  
- **Santika Sari, SP, MP** – Secondary Reviewer  

Special thanks to the **ALG research team** and everyone who provided technical or moral support during the preparation of this project.

Thank you for your valuable contributions and encouragement.

---
> 📌 **Disclaimer**  
> This repository serves as a simplified technical documentation of the author's undergraduate thesis.  
> It is **not intended as a formal academic publication**, and does not substitute for peer-reviewed or published works.  
> Any reproduction, citation, or reuse of this repository for academic or commercial purposes should be done with proper credit to the author.

# Peluang Kekeringan Berdasarkan Karakteristik Suhu Permukaan, Kehijauan Vegetasi, dan Presipitasi di Sub DAS Cikapundung

Penelitian ini bertujuan untuk menganalisis peluang kejadian kekeringan dengan pendekatan spasial dan statistik berdasarkan tiga parameter utama, yaitu suhu permukaan, keragaman vegetasi (NDVI), dan presipitasi. Studi kasus dilakukan pada wilayah Sub DAS Cikapundung, Lembang.

## 👤 Penulis

**Miftahul Ardli**  
NIM: 150510180225  
Program Studi Agroteknologi
Departemen Ilmu Tanah dan Sumber Daya Lahan
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
## ⚡ Bonus: Model XGBoost

Sebagai pelengkap dari model utama **Random Forest**, proyek ini juga menyertakan implementasi eksperimental dari algoritma **XGBoost** (*Extreme Gradient Boosting*) untuk membandingkan performa dalam prediksi kekeringan.

**XGBoost** dikenal karena kecepatannya dan akurasi tinggi dalam tugas regresi, serta banyak digunakan dalam kompetisi data science maupun aplikasi nyata. Meskipun model **Random Forest** memberikan hasil terbaik dalam studi ini, keberadaan **XGBoost** berperan sebagai tolok ukur tambahan yang memperkaya perbandingan performa model.

---

## 🙏 Ucapan Terima Kasih

Proyek ini merupakan bagian dari tugas akhir yang disusun untuk memperoleh gelar Sarjana Pertanian di Universitas Padjadjaran. Penulis menyampaikan terima kasih sebesar-besarnya kepada pihak-pihak yang telah membimbing dan memberikan arahan selama proses penelitian dan pengembangan proyek ini.

Ucapan terima kasih khusus kepada:

- **Prof. Dr. Ir. H. Mahfud Arifin, MS** – selaku Ketua Komisi Pembimbing, atas bimbingan, arahan, dan motivasi yang konsisten selama penyusunan skripsi dan proyek ini.

- **Dr. Muhammad Amir Solihin, SP, MT** – selaku Anggota Komisi Pembimbing dan Ketua Program Studi Agroteknologi, atas masukan mendalam terkait metode dan kontribusinya dalam pengembangan penelitian.

- **Ade Setiawan, SP, MP** – selaku Ketua Komisi Penelaah, atas kritik dan saran yang membangun dalam penyempurnaan karya ilmiah ini.

- **Santika Sari, SP, MP** – selaku Anggota Komisi Penelaah, atas perhatian dan koreksi yang sangat membantu dalam meningkatkan kualitas hasil akhir.

Penulis juga mengucapkan terima kasih kepada seluruh rekan di tim penelitian ALG dan semua pihak yang telah mendukung, baik secara teknis maupun moral, selama proses pengerjaan proyek ini.

Terima kasih atas segala kontribusi dan dukungannya. 🙏

> 📌 **Disclaimer**  
> Repositori ini merupakan dokumentasi teknis sederhana dari tugas akhir penulis (skripsi).  
> Repositori ini **bukan merupakan publikasi ilmiah resmi**, dan tidak dimaksudkan sebagai pengganti karya yang telah ditinjau sejawat atau diterbitkan secara formal.  
> Setiap penggunaan ulang, kutipan, atau reproduksi untuk keperluan akademik maupun komersial harus disertai dengan atribusi yang sesuai kepada penulis.
