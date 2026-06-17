# Clustering

## Pengertian

Clustering adalah teknik untuk mengelompokkan data atau objek berdasarkan kriteria kemiripan tertentu. Tujuan clustering adalah mengelompokkan n data ke dalam k cluster, di mana k < n dan k > 0. Data dalam satu cluster memiliki kemiripan tinggi, sedangkan data antar cluster memiliki perbedaan yang signifikan.

Kriteria kemiripan ditentukan oleh:
- **Atribut yang digunakan** (misalnya: warna, ukuran, tinggi, jari-jari)
- **Jarak antar data** (berdasarkan rumus jarak tertentu)
- **Struktur dan bentuk cluster** yang diharapkan

## Rumus Jarak (Distance Measures)

Clustering berbasis jarak menggunakan perhitungan kemiripan antar objek berdasarkan rumus jarak. Rumus jarak mempengaruhi bentuk cluster yang terbentuk.

### Jarak Minkowski
Rumus umum untuk menghitung jarak dengan order parameter p:
- Dikenal sebagai **L-p norm**
- Dengan nilai p yang berbeda menghasilkan rumus jarak yang berbeda

### Jenis Jarak Minkowski:

**p = 1 (L1 norm):**
- **Jarak Manhattan** (city block): Jumlah perbedaan absolut di setiap dimensi
- **Jarak Hamming**: Jumlah bit yang berbeda antara dua vektor biner

**p = 2 (L2 norm):**
- **Jarak Euclidean**: Akar kuadrat dari jumlah kuadrat perbedaan (garis lurus/distance as the crow flies)

**p = ∞ (Lmax norm):**
- **Jarak Supremum/Maksimum**: Perbedaan maksimum di antara semua atribut pada vektor

### Jarak Lainnya:
- **Jarak Cosine**: Mengukur sudut antar vektor, sering digunakan untuk data text/dokumen
- Rumus jarak dipilih sesuai dengan sifat data dan kebutuhan aplikasi

## Dua Tipe Clustering Berbasis Jarak

### 1. Algoritma Partisi
Menyusun beberapa partisi dan mengevaluasinya menggunakan kriteria tertentu.

Algoritma utama:
- **K-Means**: Mengelompokkan data dengan meminimalkan sum of squares of distance
- **K-Medoids**: Menggunakan data point sebagai representative
- **K-Median**: Menggunakan median data dalam cluster
- **Fuzzy C-Means**: Soft clustering dengan membership fuzzy

### 2. Algoritma Hirarki
Membuat dekomposisi hirarki dari kumpulan objek menggunakan kriteria tertentu.

**Agglomerative** ("bottom-up"):
- Dimulai dengan menjadikan setiap objek sebagai satu cluster
- Selanjutnya menggabungkannya menjadi cluster yang lebih besar
- Proses berlanjut sampai semua objek menjadi satu cluster

**Divisive** ("top-down"):
- Dimulai dari satu cluster yang besar
- Selanjutnya membagi menjadi cluster-cluster yang lebih kecil
- Proses berlanjut sampai setiap objek menjadi cluster sendiri

## Algoritma K-Means

### Konsep

K-Means adalah algoritma untuk mengelompokkan n objek/data berdasarkan atribut/fitur ke dalam k cluster, dengan asumsi bahwa atribut objek membentuk suatu ruang vektor (vector space).

Pengelompokan dilakukan dengan **meminimalkan sum of squares of distance (J)** antara objek dengan pusat clusternya (centroid).

### Alur Algoritma K-Means

**Langkah 1:** Tentukan nilai k = jumlah cluster yang diinginkan.

**Langkah 2:** Tentukan k centroid awal dengan memilih k data secara random.
- Bisa dipilih k data pertama sebagai centroid
- Atau k data terjauh sebagai centroid (lebih baik untuk konvergensi)

**Langkah 3:** Hitung jarak Euclidean tiap data ke setiap centroid.

**Langkah 4:** Masukkan setiap data ke dalam cluster dengan jarak centroid terdekat.

**Langkah 5:** Hitung ulang nilai centroid menggunakan rata-rata (mean) data dalam suatu cluster.

**Langkah 6:** Ulangi langkah 3, 4, 5 sampai konvergen (tidak ada lagi perpindahan objek dari satu cluster ke cluster lain).

### Visualisasi Proses

Algoritma K-Means dapat divisualisasikan sebagai:
```
Mulai
  ↓
Tentukan k, Inisialisasi centroid
  ↓
Hitung jarak objek ke centroid
  ↓
Kelompokkan objek ke cluster dengan jarak centroid minimum
  ↓
Masih ada perpindahan? → Ya → Hitung ulang posisi centroid → [kembali ke langkah sebelumnya]
  ↓ Tidak
Hasil cluster
  ↓
Berhenti
```

### Contoh K-Means dengan k=2

Data dengan atribut (jari-jari, tinggi):
- 11 data point tersedia
- Inisialisasi dengan 2 data pertama sebagai centroid
- m1 = (1.0, 2.0), m2 = (1.1, 2.0)

**Iterasi 1:**
- Hitung jarak Euclidean setiap data ke kedua centroid
- Kelompokkan ke cluster terdekat
- Hitung ulang centroid berdasarkan mean data dalam cluster
- Hasilnya: Cluster 1 = {1,3,4,5,6,7,8}, Cluster 2 = {2,9,10,11}

**Iterasi 2:**
- Ulangi proses dengan centroid baru
- Periksa apakah masih ada perpindahan data
- Jika tidak ada perpindahan, algoritma konvergen dan selesai

## Contoh Aplikasi Clustering

### Segmentasi Pembeli (Customer Segmentation)
1. **Identifikasi** kelompok pembeli potensial untuk penjualan produk
2. **Implementasi** algoritma clustering untuk mengelompokkan pembeli berdasarkan perilaku/karakteristik
3. **Aksi** Jual produk ke setiap segmen pembeli dengan strategi yang disesuaikan

### Aplikasi Lainnya
- **Rekomendasi sistem** berbasis hierarchical clustering untuk e-learning
- **Identifikasi pola** dalam data besar
- **Pengelompokan dokumen** (document clustering)
- **Analisis pasar** dan tren konsumen

## Inti Kesimpulan

Clustering adalah teknik unsupervised learning yang menggunakan perhitungan jarak untuk mengelompokkan data. Dua pendekatan utama adalah **partisi** (K-Means, lebih cepat) dan **hirarki** (menghasilkan dendrogram). Pemilihan rumus jarak dan algoritma tergantung pada sifat data dan kebutuhan aplikasi.
