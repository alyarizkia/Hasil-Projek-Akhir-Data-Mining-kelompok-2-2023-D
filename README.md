# **🔍 Analisis Pola Kriminalitas Spatio-Temporal Menggunakan Association Rule Mining dengan Apriori dan FP-Growth**
# **Kelompok 2:**
1. Sheira En Nadia (23031554041)
2. Salsabila Rinita Candraningtyas (23031554179)
3. Fakhriatu J Koni (23031554186)
4. Alya' Hikmatul Rizkia (23031554229)

# **Deskripsi Proyek**
Melakukan analisa pola kriminalitas dengan menggunakan Association Rule Mining (ARM) dengan menggunakan algoritma Apriori dan FP-Growth. Tujuannya untuk membantu pihak berwenang untuk mengenali pola-pola kriminalitas berdasarkan lokasi dan waktu, serta memberikan wawasan mengenai efektivitas algoritma Apriori dan FP-Growth dalam membuat pola.

# **Tools yang Digunakan**
1. Python
2. Pandas
3. Numpy
4. Mixtend
5. Seaborn
6. Matplotlib

# **Dataset**
Menggunakan dataset yang diambil dari [website Kota Chicago](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/data_preview)

# **Langkah Pengerjaan**
## 1. Data Pre-processing
- Data Cleaning: Menghapus duplikasi, memperbaiki nilai kosong, dan membuang atribut yang tidak relevan.
- Transformasi Atribut: Ekstraksi elemen tanggal menjadi bulan, hari dalam minggu, dan jam.
- Encoding Data: Konversi atribut kategorikal menjadi format numerik agar dapat diproses oleh algoritma mining.

## 2. Association Rule Mining
- Algortima Apriori: Menerapkan algoritma Apriori untuk mencari frequent itemsets berdasarkan threshold minimum support dan minimum confidence.
- Algortima FP-Growth: Menerapkan algoritma FP-Growth untuk menghasilkan frequent itemsets lebih cepat dengan membangun FP-Tree, sehingga lebih efisien untuk dataset besar.

## 3. Evaluasi dan Perbandingan Algoritma
Membandingkan hasil yang diperoleh dari kedua algoritma berdasarkan:
- Jumlah rule yang dihasilkan,
- Waktu komputasi,
- Nilai support, confidence, dan lift.  

## 4. Analisis Pola Kriminalitas
- Menginterpretasikan pola-pola asosiasi yang ditemukan, mengidentifikasi waktu-waktu rawan, lokasi berisiko tinggi, serta keterkaitan jenis kejahatan dengan faktor spasial dan temporal.
- Menyimpulkan hasil analisis dan memberikan rekomendasi strategis untuk pencegahan dan penanganan kejahatan di masa depan berbasis data.

# 📊 3 Pola-Pola Teratas yang Dihasilkan
- Apriori:
  1. Jika terjadi kasus kriminalitas berupa penggunaan narkotika, maka itu terjadi pada bulan April dan terjadi penangkapan pada pelaku
  2. Jika terjadi kasus kriminalitas berupa kecanduan narkotika pada bulan april, maka pelaku tersebut ditangkap
  3. Jika terjadi kasus kriminalitas ketergantungan narkotika, maka itu terjadi pada tahun 2025 dan pelakunya ditangkap

- FP-Growth:
  1. Jika terjadi kasus kriminalitas berupa penggunaan narkotika, maka kasus itu hampir pasti terjadi pada bulan April di tahun 2025 dan terjadi penangkapan pada pelaku
  2. Jika terjadi kasus kriminalitas berupa kecanduan narkotika, besar kemungkinan pelaku tersebut ditangkap
  3. Jika terjadi kasus kriminalitas ketergantungan narkotika pada bulan April, maka terdapat kemungkinan pelaku tersebut tertangkap oleh pihak berwajib

# Referensi
Sevri, M., Karacan, H., & Akcayol, M. A. (2017). Crime analysis based on association rules using apriori algorithm. International Journal of Information and Electronics Engineering, 7(3), 99-102.
