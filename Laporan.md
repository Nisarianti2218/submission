# Laporan Proyek Machine Learning – Nisa Rianti

## Domain Proyek

Kanker payudara merupakan salah satu jenis kanker paling umum dan menjadi penyebab utama kematian akibat kanker pada wanita di seluruh dunia. Deteksi dini serta diagnosis yang akurat menjadi faktor kunci untuk meningkatkan peluang kesembuhan dan kelangsungan hidup pasien. Salah satu metode diagnostik yang sering digunakan adalah *Fine Needle Aspiration* (FNA), yaitu prosedur pengambilan sampel sel dari jaringan payudara menggunakan jarum halus untuk dianalisis secara mikroskopis. Karakteristik inti sel, seperti ukuran radius, tekstur, perimeter, dan area, dapat memberikan petunjuk penting mengenai sifat sel tersebut—apakah bersifat jinak (*benign*) atau ganas (*malignant*).

Proyek ini bertujuan untuk membangun model *machine learning* yang mampu mengklasifikasikan hasil diagnosis kanker payudara berdasarkan fitur-fitur numerik yang diekstraksi dari citra digital hasil prosedur FNA. Dengan memanfaatkan teknologi pembelajaran mesin, sistem ini diharapkan dapat menjadi alat bantu diagnosis yang objektif, cepat, dan akurat bagi tenaga medis.

### Alasan dan Metode Penyelesaian Masalah

Proses diagnosis kanker payudara secara manual melalui pengamatan mikroskopis kerap kali bersifat subjektif dan memakan waktu. Kesalahan dalam diagnosis, baik *false positive* (mendiagnosis ganas padahal jinak) maupun *false negative* (mendiagnosis jinak padahal ganas), dapat berdampak serius. *False positive* dapat menyebabkan stres emosional dan intervensi medis yang tidak diperlukan, sedangkan *false negative* bisa berujung pada keterlambatan penanganan medis yang krusial.

Teknik *machine learning* memiliki keunggulan dalam mengidentifikasi pola-pola kompleks dari data numerik yang sulit ditangkap secara kasat mata oleh manusia. Dengan melatih model pada dataset historis dengan label yang telah diverifikasi, kita dapat mengembangkan sistem prediktif yang:

- Menyediakan diagnosis yang lebih akurat.
- Mengurangi ketergantungan pada subjektivitas pengamat.
- Mempercepat proses pengambilan keputusan.
- Memberikan *second opinion* berbasis data untuk membantu ahli patologi.

## Referensi

1. World Health Organization (WHO). (2023). *Breast cancer*. [Tersedia online](https://www.who.int/news-room/fact-sheets/detail/breast-cancer)
2. Street, W. N., Wolberg, W. H., & Mangasarian, O. L. (1993). Nuclear feature extraction for breast tumor diagnosis. *IS&T/SPIE's Symposium on Electronic Imaging: Science & Technology*, *1905*, 861–870. San Jose, CA. [https://doi.org/10.1117/12.148698](https://doi.org/10.1117/12.148698)
3. Wolberg, W., Mangasarian, O., Street, N., & Street, W. (1993). Breast Cancer Wisconsin (Diagnostic) [Dataset]. UCI Machine Learning Repository. [https://doi.org/10.24432/C5DW2B](https://doi.org/10.24432/C5DW2B)


## Domain Proyek

Kanker payudara adalah salah satu jenis kanker yang paling sering terjadi dan menjadi penyebab utama kematian akibat kanker pada wanita di seluruh dunia. Deteksi secara dini dan diagnosis yang tepat sangat penting untuk meningkatkan harapan hidup serta peluang pemulihan pasien. Salah satu prosedur yang umum digunakan dalam diagnosis adalah *Fine Needle Aspiration* (FNA), yakni teknik pengambilan sampel sel dari benjolan di payudara untuk kemudian dianalisis di bawah mikroskop. Ciri-ciri inti sel seperti radius, tekstur, perimeter, dan area dapat digunakan untuk mengklasifikasikan apakah sel tersebut tergolong jinak (*benign*) atau ganas (*malignant*).

Tujuan utama proyek ini adalah merancang model *machine learning* yang mampu mengklasifikasikan diagnosis kanker payudara berdasarkan fitur-fitur yang diperoleh dari hasil FNA. Dengan pendekatan ini, diharapkan dapat tercipta sistem pendukung keputusan medis yang bersifat objektif, akurat, dan efisien untuk membantu para profesional kesehatan dalam membuat diagnosis.

### Alasan Pentingnya Permasalahan Ini

Diagnosis kanker payudara secara manual melalui observasi mikroskopis cenderung subjektif dan membutuhkan waktu yang tidak sedikit. Kesalahan diagnosis seperti *false positive* (menyatakan ganas padahal jinak) dapat menyebabkan kecemasan dan prosedur medis yang tidak perlu, sementara *false negative* (menyatakan jinak padahal ganas) dapat menunda pengobatan yang penting.

Dengan bantuan *machine learning*, kita dapat menganalisis data fitur sel secara mendalam dan mengungkap pola-pola kompleks yang mungkin luput dari pengamatan manusia. Melatih model menggunakan dataset historis dengan label diagnosis yang telah diverifikasi memungkinkan pembangunan sistem prediktif yang dapat:
- Meningkatkan ketepatan diagnosis.
- Mengurangi ketergantungan pada subjektivitas manusia.
- Mempercepat proses penilaian medis.
- Memberikan pandangan alternatif (second opinion) berbasis data untuk mendukung keputusan dokter.

### Referensi:
1. World Health Organization (WHO). (2023). *Breast cancer*. [https://www.who.int/news-room/fact-sheets/detail/breast-cancer](https://www.who.int/news-room/fact-sheets/detail/breast-cancer)  
2. Street, W. N., Wolberg, W. H., & Mangasarian, O. L. (1993). *Nuclear feature extraction for breast tumor diagnosis*. *IS&T/SPIE Symposium on Electronic Imaging*, *1905*, 861–870. [https://doi.org/10.1117/12.148698](https://doi.org/10.1117/12.148698)  
3. Wolberg, W., Mangasarian, O., Street, N., & Street, W. (1993). *Breast Cancer Wisconsin (Diagnostic) Dataset*. UCI Machine Learning Repository. [https://doi.org/10.24432/C5DW2B](https://doi.org/10.24432/C5DW2B)

---

## Business Understanding

Proyek ini bertujuan untuk memanfaatkan data hasil biopsi FNA guna membangun model prediktif yang mampu membantu proses diagnosis kanker payudara secara lebih akurat dan efisien.

### Rumusan Masalah
- Bagaimana membangun model *machine learning* yang mampu mengklasifikasikan tumor payudara sebagai jinak (*benign*) atau ganas (*malignant*) berdasarkan fitur-fitur yang diperoleh dari sampel sel?
- Di antara algoritma Logistic Regression, Decision Tree, dan Random Forest, mana yang menghasilkan performa terbaik berdasarkan metrik evaluasi seperti akurasi, presisi, dan recall?
- Fitur-fitur apa saja yang paling berkontribusi dalam membedakan tumor jinak dan ganas?

### Tujuan Proyek
- Mengembangkan model klasifikasi kanker payudara dengan tingkat akurasi tinggi.
- Melakukan evaluasi dan perbandingan performa tiga algoritma klasifikasi: Logistic Regression, Decision Tree, dan Random Forest, menggunakan metrik akurasi, presisi, recall, dan F1-score.
- Menentukan fitur-fitur paling signifikan dalam memprediksi diagnosis untuk memberikan wawasan yang bernilai secara klinis.

### Pernyataan Solusi

- **Solusi 1: Pengembangan dan Evaluasi Model Klasifikasi**  
  Membangun dan melatih tiga model machine learning (Logistic Regression, Decision Tree, dan Random Forest) menggunakan dataset Breast Cancer Wisconsin. Evaluasi kinerja dilakukan menggunakan metrik akurasi, presisi, recall, dan F1-score. Selain itu, digunakan juga kurva ROC dan AUC untuk menilai kemampuan klasifikasi model secara menyeluruh. Model dengan performa terbaik akan dipilih sebagai solusi utama.

- **Solusi 2: Identifikasi Fitur yang Paling Berpengaruh**  
  Setelah model terbaik ditentukan, dilakukan analisis terhadap fitur-fitur yang paling berpengaruh terhadap hasil prediksi. Untuk model pohon seperti Random Forest, fitur penting dapat diukur melalui atribut `feature_importances_`, sementara untuk Logistic Regression digunakan analisis koefisien model. Informasi ini juga diperkuat dengan hasil eksplorasi data awal (EDA) yang dilakukan sebelumnya untuk memberikan pemahaman yang lebih baik terhadap faktor biologis yang relevan dalam proses klasifikasi.


## Data Understanding

Dataset yang digunakan dalam proyek ini adalah **Breast Cancer Wisconsin (Diagnostic) Dataset**, yang diperoleh dari UCI Machine Learning Repository dan juga tersedia melalui platform Kaggle. Pada proyek ini, data dimuat dari file `data.csv`.

🔗 **Tautan Dataset Kaggle:**  
[https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

Dataset ini berisi fitur-fitur yang dihitung dari citra digital hasil prosedur Fine Needle Aspiration (FNA) dari benjolan di payudara. Fitur-fitur tersebut menggambarkan karakteristik inti sel dalam gambar mikroskopis. Contoh visual dari citra tersebut tersedia di:  
[http://www.cs.wisc.edu/~street/images/](http://www.cs.wisc.edu/~street/images/)

Pada konteks aslinya, bidang pemisah (separating plane) untuk klasifikasi diperoleh menggunakan metode *Multisurface Method-Tree* (MSM-T), yaitu teknik klasifikasi berbasis *linear programming* yang menghasilkan pohon keputusan. Pemilihan fitur dilakukan melalui pencarian menyeluruh dalam ruang kombinasi 1-4 fitur dan 1-3 bidang pemisah.

📘 **Referensi Metodologi Klasifikasi:**  
K. P. Bennett & O. L. Mangasarian, *"Robust Linear Programming Discrimination of Two Linearly Inseparable Sets"*, Optimization Methods and Software, 1992.  
[http://dx.doi.org/10.1080/10556789208805504](http://dx.doi.org/10.1080/10556789208805504)

### Struktur Dataset
Dataset ini terdiri dari **569 baris (sampel)** dan **32 kolom**, yang mencakup:
- **id**: ID unik untuk setiap pasien.
- **diagnosis**: Label target, yang menunjukkan hasil diagnosis kanker:
  - `'M'`: Malignant (ganas)
  - `'B'`: Benign (jinak)
- **30 fitur numerik**: Merupakan hasil pengukuran karakteristik inti sel, dihitung dari citra digital hasil FNA. Untuk setiap karakteristik seluler, terdapat tiga jenis pengukuran:
  - `*_mean`: Nilai rata-rata
  - `*_se`: Standar error
  - `*_worst`: Nilai maksimum atau paling ekstrem

Fitur-fitur yang diamati meliputi:
- `radius`: Jari-jari rata-rata inti sel
- `texture`: Tekstur (standar deviasi nilai skala abu-abu)
- `perimeter`: Keliling inti sel
- `area`: Luas inti sel
- `smoothness`: Tingkat kehalusan (variasi lokal jari-jari)
- `compactness`: Kekompakan (rumus: perimeter² / area - 1.0)
- `concavity`: Tingkat kecekungan kontur
- `concave points`: Jumlah titik cekung
- `symmetry`: Tingkat simetri sel
- `fractal_dimension`: Dimensi fraktal (mengukur kerumitan bentuk sel)

### 📌 Contoh Kode Python untuk Melihat Kolom Dataset

```python
import pandas as pd

# Membaca dataset
df = pd.read_csv('dataset/data.csv')

# Menampilkan daftar kolom
print(df.columns.tolist())
Outputnya adalah: `['id', 'diagnosis', 'radius_mean', 'texture_mean', 'perimeter_mean', 'area_mean', 'smoothness_mean', 'compactness_mean', 'concavity_mean', 'concave points_mean', 'symmetry_mean', 'fractal_dimension_mean', 'radius_se', 'texture_se', 'perimeter_se', 'area_se', 'smoothness_se', 'compactness_se', 'concavity_se', 'concave points_se', 'symmetry_se', 'fractal_dimension_se', 'radius_worst', 'texture_worst', 'perimeter_worst', 'area_worst', 'smoothness_worst', 'compactness_worst', 'concavity_worst', 'concave points_worst', 'symmetry_worst', 'fractal_dimension_worst']`


### Exploratory Data Analysis (EDA)
Tahapan EDA dilakukan untuk memahami data lebih dalam.
- **Pengecekan Nilai Hilang dan Duplikat:** Hasil pemeriksaan menunjukkan bahwa tidak ada nilai hilang maupun data duplikat dalam dataset ini, menandakan kualitas data yang baik.
- **Statistik Deskriptif:**
    - Dataset memiliki 569 observasi.
    - Fitur `id` tidak akan digunakan untuk pemodelan.
    - Fitur-fitur `_mean`, `_se`, dan `_worst` menunjukkan variasi nilai yang cukup besar, dengan fitur `_worst` umumnya memiliki nilai rata-rata dan maksimum yang lebih tinggi.
    - Beberapa fitur seperti `concavity_mean` dan `concave points_mean` memiliki nilai minimum 0.00.
    - Adanya perbedaan signifikan antara Q3 dan nilai maksimum pada beberapa fitur (misalnya `area_mean`) mengindikasikan potensi adanya outliers atau distribusi data yang miring.
- **Analisis Variabel Target (`diagnosis`):**
    - Kelas 'B' (Benign): 357 sampel (62.7%).
    - Kelas 'M' (Malignant): 212 sampel (37.3%).
    - Terdapat ketidakseimbangan kelas yang moderat.
    - Variabel target ini kemudian diubah menjadi numerik ('M': 1, 'B': 0) untuk keperluan visualisasi dan pemodelan.

- **Visualisasi Distribusi Target:**
  ![Visualisasi Distribusi Target](![alt text](image-1.png))
  Count plot dan pie chart digunakan untuk memvisualisasikan distribusi kelas target, yang mengkonfirmasi proporsi 62.7% Benign dan 37.3% Malignant.

```python
# # Contoh kode untuk visualisasi distribusi target (setelah mapping ke numerik)
if df[target_col].dtype == 'object':
  target_mapping = {'M': 1, 'B': 0}
  df[target_col] = df[target_col].map(target_mapping)
  sns.countplot(data=df, x=target_col)
  plt.title('Distribusi Kelas Target')
  plt.show()
```

- **Analisis Korelasi Fitur:**
![Analisis Korelasi Fitur](![alt text](image-2.png))
    - Heatmap korelasi menunjukkan adanya multikolinearitas yang tinggi antar fitur-fitur yang berkaitan dengan ukuran dan bentuk sel (misalnya, `radius_mean`, `perimeter_mean`, `area_mean`).
    - 10 fitur dengan korelasi absolut tertinggi terhadap variabel target (`diagnosis`) diidentifikasi, dengan `concave points_worst`, `perimeter_worst`, dan `concave points_mean` menempati posisi teratas.
    - Visualisasi distribusi dua fitur teratas (`concave points_worst` dan `perimeter_worst`) berdasarkan kelas target menunjukkan pemisahan yang cukup jelas, di mana nilai yang lebih tinggi cenderung berasosiasi dengan diagnosis Malignant.


## Data Preparation  
Proses persiapan data dilakukan untuk memastikan dataset siap dan optimal digunakan dalam pemodelan machine learning.

1. **Pemisahan Fitur dan Target**  
Dataset dipisahkan menjadi matriks fitur `X` yang berisi semua fitur numerik yang relevan (`numeric_features`), dan vektor target `y` berdasarkan kolom target (`target_col`).  
```python
X = df[numeric_features]
y = df[target_col]
**Alasan:**Memisahkan fitur dan target adalah langkah standar dalam supervised learning agar model dapat belajar memetakan fitur ke target. Dengan mengetahui dimensi fitur dan target, kita juga bisa memastikan bahwa data sudah sesuai untuk proses berikutnya.

2. **Pembagian Data (Train-Test Split)**  
Data dibagi menjadi set pelatihan (80%) dan set pengujian (20%) menggunakan train_test_split dengan stratifikasi berdasarkan target y dan random_state=42 untuk memastikan hasil yang konsisten.
```python
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42, stratify=y
)
**Alasan:**Pembagian ini penting untuk evaluasi model secara objektif pada data yang belum pernah dilihat. Stratifikasi memastikan proporsi kelas tetap seimbang di kedua set, sehingga model dapat belajar dengan baik pada kelas minoritas maupun mayoritas.

3. **Standarisasi Fitur (Feature Scaling)**  
Fitur numerik pada data training distandarisasi menggunakan StandardScaler, dan transformasi yang sama diterapkan ke data testing. Scaler hanya di-fit pada data training agar tidak terjadi kebocoran data (data leakage).
```python
scaler = StandardScaler()
X_train_scaled = scaler.fit_transform(X_train)
X_test_scaled = scaler.transform(X_test)
**Alasan:**Standarisasi mengubah fitur agar memiliki rata-rata 0 dan standar deviasi 1. Ini sangat membantu algoritma yang sensitif terhadap skala, seperti Logistic Regression. Selain itu, standarisasi mempercepat proses pelatihan dan memastikan setiap fitur berkontribusi secara seimbang.

3. **Verifikasi dan Informasi Tambahan**  
- Menampilkan dimensi fitur dan target untuk memastikan data sudah benar.
- Menampilkan dimensi data training dan testing untuk konfirmasi split.
- Mengecek distribusi nilai rata-rata dan standar deviasi fitur sebelum dan sesudah scaling untuk validasi proses standarisasi.
- Memastikan distribusi proporsi kelas pada training dan testing tetap terjaga setelah split.
```python
print(f"Dimensi fitur (X): {X.shape}")
print(f"Dimensi target (y): {y.shape}")

print(f"\nData training: {X_train.shape}")
print(f"Data testing: {X_test.shape}")

print(f"\nStandarisasi selesai!")
print(f"Mean sebelum scaling (sample): {X_train.iloc[:, 0].mean():.3f}")
print(f"Mean setelah scaling (sample): {X_train_scaled[:, 0].mean():.3f}")
print(f"Std setelah scaling (sample): {X_train_scaled[:, 0].std():.3f}")

print(f"\nDistribusi kelas di training set:")
print(y_train.value_counts(normalize=True))
print(f"\nDistribusi kelas di testing set:")
print(y_test.value_counts(normalize=True))

Hasil akhir dari proses ini adalah data yang sudah dipisah dengan benar, di-split secara proporsional, dan fitur yang distandarisasi, sehingga siap digunakan untuk melatih model machine learning dengan evaluasi yang valid dan handal.

## Modeling  
Tiga algoritma klasifikasi machine learning diterapkan dan dilatih untuk memprediksi diagnosis kanker payudara.

1. **Logistic Regression**  
   - **Proses:** Model Logistic Regression dibuat dengan parameter `random_state=42` untuk memastikan hasil yang dapat direplikasi, serta `max_iter=1000` untuk memastikan proses pelatihan mencapai konvergensi. Model ini dilatih menggunakan fitur yang sudah distandarisasi (`X_train_scaled`) dan target (`y_train`).  
   - **Parameter:** `random_state=42`, `max_iter=1000`.  
   - **Kelebihan:** Cepat dalam pelatihan, mudah dipahami karena koefisiennya menunjukkan pengaruh fitur, dapat memberikan probabilitas prediksi, dan sering digunakan sebagai baseline.  
   - **Kekurangan:** Mengasumsikan hubungan linear antara fitur dan log-odds target, sehingga performanya bisa menurun pada data dengan pola non-linear kompleks.  

2. **Decision Tree Classifier**  
   - **Proses:** Model Decision Tree dibuat dengan `random_state=42` dan `max_depth=10` untuk membatasi kedalaman pohon, guna menghindari overfitting yang berlebihan. Model dilatih menggunakan fitur asli tanpa scaling (`X_train`) dan target (`y_train`).  
   - **Parameter:** `random_state=42`, `max_depth=10`.  
   - **Kelebihan:** Mudah diinterpretasikan karena strukturnya yang intuitif, mampu menangani pola non-linear antar fitur, dan tidak membutuhkan standarisasi fitur.  
   - **Kekurangan:** Rentan terhadap overfitting jika pohon terlalu dalam, serta model bisa tidak stabil karena perubahan kecil di data dapat menghasilkan pohon yang berbeda.  

3. **Random Forest Classifier**  
   - **Proses:** Model Random Forest terdiri dari banyak pohon keputusan, diinisialisasi dengan `random_state=42` dan jumlah pohon `n_estimators=100`. Model ini juga dilatih pada data fitur asli (`X_train`) dan target (`y_train`).  
   - **Parameter:** `random_state=42`, `n_estimators=100`.  
   - **Kelebihan:** Biasanya memberikan akurasi yang baik, lebih tahan terhadap overfitting dibandingkan Decision Tree tunggal, mampu mengelola data dengan banyak fitur, dan menyediakan informasi pentingnya fitur.  
   - **Kekurangan:** Model lebih kompleks dan kurang transparan dibandingkan Decision Tree tunggal, serta membutuhkan waktu komputasi yang lebih lama saat pelatihan.  

**Hasil Akurasi pada Data Training:**  
- Logistic Regression: 0.9868  
- Decision Tree: 1.0000  
- Random Forest: 1.0000  

Akurasi 100% pada Decision Tree dan Random Forest menandakan kemungkinan model mengalami *overfitting*. Oleh sebab itu, evaluasi pada data testing penting untuk menguji kemampuan generalisasi model.

---

### Analisis Feature Importance  

Untuk memahami fitur-fitur yang paling berpengaruh dalam prediksi, dilakukan analisis *feature importance* pada model Decision Tree dan Random Forest.

**Top 10 fitur penting pada Decision Tree:**  
1. `perimeter_worst`: 0.7232  
2. `concave points_worst`: 0.0677  
3. `smoothness_worst`: 0.0408  
4. `texture_mean`: 0.0292  
5. `area_mean`: 0.0225  
6. `texture_worst`: 0.0187  
7. `area_worst`: 0.0156  
8. `concavity_worst`: 0.0143  
9. `fractal_dimension_worst`: 0.0134  
10. `texture_se`: 0.0125  

**Top 10 fitur penting pada Random Forest:**  
1. `area_worst`: 0.1310  
2. `perimeter_worst`: 0.1303  
3. `concave points_worst`: 0.1032  
4. `radius_worst`: 0.0978  
5. `concave points_mean`: 0.0874  
6. `area_mean`: 0.0584  
7. `perimeter_mean`: 0.0484  
8. `concavity_worst`: 0.0478  
9. `area_se`: 0.0419  
10. `concavity_mean`: 0.0366  

Visualisasi fitur teratas pada kedua model dapat dilihat pada gambar berikut:  
![Feature Importance Decision Tree dan Random Forest](![alt text](image-3.png))  

**Interpretasi:**  
Setelah model-model berhasil dilatih, langkah berikutnya adalah menganalisis **feature importance** untuk mengetahui fitur mana yang paling berpengaruh dalam pengambilan keputusan model. Analisis ini penting untuk interpretabilitas model sekaligus validasi klinis.

### Feature Importance pada Model Decision Tree:

- **perimeter_worst (72.32%)**  
  Fitur ini mendominasi secara signifikan dalam klasifikasi Decision Tree, menandakan bahwa keliling area terburuk dari massa tumor adalah faktor utama dalam membedakan tumor jinak dan ganas.

- **concave points_worst (6.77%)**  
  Jumlah titik cekung terburuk, mencerminkan kompleksitas bentuk tumor, menjadi fitur penting kedua.

- **smoothness_worst (4.08%)**  
  Tingkat kehalusan permukaan tumor dalam kondisi terburuk juga berkontribusi signifikan.

- **Fitur lain**  
  Sisa fitur memiliki kontribusi kecil (< 3% masing-masing).

### Feature Importance pada Model Random Forest:

- **area_worst (13.10%)**  
  Area terburuk menjadi fitur terpenting, menunjukkan ukuran tumor sangat krusial.

- **perimeter_worst (13.03%)**  
  Hampir setara dengan area_worst, mengonfirmasi pentingnya dimensi geometris tumor.

- **concave points_worst (10.32%)**  
  Konsisten dengan Decision Tree, fitur ini tetap masuk top 3.

- **radius_worst (9.78%)**  
  Radius terburuk melengkapi informasi dimensi tumor.

- **concave points_mean (8.74%)**  
  Rata-rata titik cekung juga memberikan kontribusi signifikan.


### Perbedaan Strategi Model:

1. **Decision Tree:**  
   Mengandalkan **"single dominant feature strategy"** dengan perimeter_worst sebagai splitter utama. Ini menunjukkan satu fitur geometris sudah cukup untuk klasifikasi akurat.

2. **Random Forest:**  
   Menggunakan **"ensemble wisdom approach"** yang menggabungkan informasi dari banyak fitur secara lebih seimbang. Pendekatan ini lebih robust dan komprehensif.

### Validasi Medis:

Hasil feature importance ini sangat sesuai dengan literatur medis:

- **Fitur Geometris (area, perimeter, radius):**  
  Ukuran tumor memang indikator kuat keganasan, di mana tumor ganas cenderung lebih besar dan bentuknya tidak beraturan.

- **Concave Points:**  
  Titik cekung mencerminkan **irregularitas bentuk** tumor, yang biasanya lebih kompleks pada tumor ganas.

- **Dominasi Fitur "Worst":**  
  Fitur dengan nilai ekstrem (_worst_) lebih andal dalam membedakan keganasan, karena karakteristik ekstrem seringkali lebih mencolok.

### Implikasi untuk Diagnosis Klinis:

1. **Fokus Pemeriksaan:**  
   Praktisi medis perlu menitikberatkan pada pengukuran dimensi tumor (area, perimeter, radius) dan analisis bentuk (concave points).

2. **Teknologi Imaging:**  
   Dukungan pada teknologi imaging yang mampu mengukur parameter geometris dengan presisi tinggi.

3. **Standardisasi:**  
   Pentingnya standardisasi pengukuran fitur "worst" untuk memastikan konsistensi diagnosis.


### Kesimpulan:

- **Random Forest** menunjukkan pendekatan yang **lebih robust** karena:  
  - Tidak terlalu bergantung pada satu fitur saja  
  - Menggabungkan banyak perspektif fitur  
  - Lebih tahan terhadap noise dan outlier  
  - Distribusi feature importance yang lebih natural

- **Decision Tree**, meskipun akurat, memiliki potensi **keterbatasan** karena terlalu mengandalkan satu fitur utama.

Analisis ini mengonfirmasi bahwa **karakteristik geometris tumor, terutama nilai ekstremnya, merupakan biomarker sangat kuat untuk diagnosis kanker payudara**. Temuan ini memberikan kepercayaan tinggi terhadap validitas model dan relevansi klinisnya.

## Evaluation
Evaluasi model dilakukan menggunakan data test untuk mengukur seberapa baik model dapat menggeneralisasi pada data baru. Metrik yang digunakan adalah Akurasi, Presisi, Recall, dan F1-Score. Kurva ROC dan AUC juga digunakan untuk analisis lebih lanjut.

**Penjelasan Metrik yang Digunakan:**
-   **Akurasi (Accuracy)**: Proporsi dari total prediksi yang benar (baik prediksi Benign maupun Malignant yang benar) dibagi dengan jumlah total sampel.
    -   *Formula*: `(TP + TN) / (TP + TN + FP + FN)`
    -   *Interpretasi*: Mengukur seberapa sering model membuat prediksi yang benar secara keseluruhan. Cocok untuk dataset yang seimbang.
-   **Presisi (Precision)**: Dari semua sampel yang diprediksi sebagai Malignant, berapa proporsi yang benar-benar Malignant.
    -   *Formula*: `TP / (TP + FP)`
    -   *Interpretasi*: Mengukur kemampuan model untuk tidak salah melabeli sampel Benign sebagai Malignant. Presisi tinggi penting ketika biaya False Positive tinggi.
-   **Recall (Sensitivity atau True Positive Rate)**: Dari semua sampel yang sebenarnya Malignant, berapa proporsi yang berhasil diprediksi sebagai Malignant oleh model.
    -   *Formula*: `TP / (TP + FN)`
    -   *Interpretasi*: Mengukur kemampuan model untuk menemukan semua kasus Malignant. Recall tinggi sangat krusial dalam diagnosis medis untuk meminimalkan False Negative.
-   **F1-Score**: Rata-rata harmonik dari Presisi dan Recall. Memberikan keseimbangan antara kedua metrik tersebut.
    -   *Formula*: `2 * (Precision * Recall) / (Precision + Recall)`
    -   *Interpretasi*: Berguna ketika ada ketidakseimbangan kelas atau ketika penting untuk menyeimbangkan Presisi dan Recall.
-   **ROC Curve (Receiver Operating Characteristic Curve)**: Plot yang menggambarkan kinerja model klasifikasi biner pada berbagai ambang batas klasifikasi. Kurva ini memplot True Positive Rate (Recall) terhadap False Positive Rate.
    -   *Interpretasi*: Model yang baik memiliki kurva yang mendekati sudut kiri atas.
-   **AUC (Area Under the ROC Curve)**: Mengukur keseluruhan kemampuan model untuk membedakan antara kelas positif dan negatif. Nilai AUC berkisar dari 0 hingga 1.
    -   *Interpretasi*: AUC = 1.0 berarti classifier sempurna; AUC = 0.5 berarti classifier tidak lebih baik dari tebakan acak.

Dimana:
-   TP (True Positive): Sampel Malignant yang diprediksi benar sebagai Malignant.
-   TN (True Negative): Sampel Benign yang diprediksi benar sebagai Benign.
-   FP (False Positive): Sampel Benign yang salah diprediksi sebagai Malignant (Type I Error).
-   FN (False Negative): Sampel Malignant yang salah diprediksi sebagai Benign (Type II Error).

## Evaluasi Model

| Model               | Akurasi | Precision | Recall  | F1-Score |
| :------------------ | :------ | :-------- | :------ | :------- |
| Logistic Regression | 0.9649  | 0.9750    | 0.9286  | 0.9512   |
| Decision Tree       | 0.9211  | 0.9024    | 0.8810  | 0.8916   |
| Random Forest       | 0.9561  | 1.0000    | 0.8810  | 0.9367   |

Berdasarkan nilai akurasi, **Logistic Regression tampil sebagai model terbaik** dengan akurasi tertinggi sebesar 0.9649.

Namun, jika kita meninjau performa secara menyeluruh—terutama dalam konteks diagnosis medis di mana konsekuensi *false positives* dan *false negatives* berbeda secara signifikan—beberapa hal penting perlu diperhatikan:

- **Logistic Regression** menunjukkan keseimbangan yang sangat baik antara *Precision* dan *Recall* pada kelas Malignant, sekaligus mempertahankan akurasi keseluruhan tertinggi. Ini mengindikasikan bahwa model ini efektif dalam mendeteksi sekaligus mengonfirmasi kasus Malignant dengan baik.
- **Random Forest** memiliki *Precision* sempurna (1.0000) untuk kelas Malignant, yang berarti setiap prediksi "Malignant" sangat dapat dipercaya. Hal ini sangat berguna jika biaya kesalahan positif palsu (*false positive*) sangat tinggi. Namun, *Recall* model ini sedikit lebih rendah dibanding Logistic Regression.

Secara umum, ketiga model menunjukkan performa yang sangat baik dalam tugas klasifikasi ini. Pilihan model terbaik akhirnya bergantung pada prioritas yang ingin diutamakan: apakah mengutamakan akurasi keseluruhan, meminimalkan *false positives* (Precision tinggi), atau meminimalkan *false negatives* (Recall tinggi) pada kelas Malignant. Dengan keseimbangan metrik yang dimiliki, **Logistic Regression merupakan pilihan yang sangat baik dan seimbang**.

### Analisis Confusion Matrix untuk Model Terbaik (Logistic Regression)  
![Analisis Confusion Matrix](![alt text](image-4.png))

- **True Negatives (TN)**: 70 kasus Benign yang berhasil diprediksi dengan benar.  
- **False Positives (FP)**: 1 kasus Benign yang salah diprediksi sebagai Malignant (kesalahan tipe I).  
- **False Negatives (FN)**: 3 kasus Malignant yang salah diprediksi sebagai Benign (kesalahan tipe II).  
- **True Positives (TP)**: 40 kasus Malignant yang berhasil diprediksi dengan benar.

**Interpretasi:**  
Model Logistic Regression mampu mengenali sebagian besar sampel dengan tepat, dengan jumlah kesalahan yang sangat kecil. Kesalahan prediksi yang rendah ini menunjukkan performa yang dapat diandalkan dalam membedakan antara kelas Benign dan Malignant.

### Analisis Kurva ROC dan AUC  
![Analisis Kurva ROC dan AUC](![alt text](image-5.png))

- Model Logistic Regression memiliki nilai **AUC tertinggi yaitu 0.996**, yang menandakan kemampuan diskriminasi yang sangat baik dalam membedakan antara pasien Benign dan Malignant.  
- Model Random Forest juga menunjukkan performa yang sangat baik dengan nilai **AUC 0.992**, hampir setara dengan Logistic Regression.  
- Model Decision Tree memiliki nilai **AUC terendah, yaitu 0.913**, namun masih lebih baik dibanding tebakan acak.

## **Kesimpulan Akhir:**

Visualisasi ini semakin menguatkan hasil evaluasi yang telah kita lakukan sebelumnya.

* **Logistic Regression** terus menunjukkan performa yang kuat dan seimbang di berbagai metrik, dengan nilai AUC dan *Recall* tertinggi, sehingga menjadi pilihan yang sangat andal.
* **Random Forest** juga menunjukkan hasil yang sangat baik, khususnya dengan *Precision* sempurna (tanpa *False Positives*), yang sangat penting dalam aplikasi medis. Namun, *Recall*-nya sedikit di bawah Logistic Regression.
* **Decision Tree** tampil lebih rendah dibanding kedua model lainnya di semua metrik, menandakan model ini kurang mampu melakukan generalisasi pada data baru.

Dari analisis menyeluruh ini, **Logistic Regression dan Random Forest merupakan model terbaik dan paling potensial** untuk tugas klasifikasi diagnosis kanker payudara.
