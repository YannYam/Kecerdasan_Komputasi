# Catatan Materi: Computational Intelligence (Kecerdasan Komputasional)

## 📌 Bentuk-Bentuk Utama
Terdapat beberapa metode utama dalam sistem kecerdasan ini:
* **Neural Network** (Jaringan Saraf Tiruan)
* **Fuzzy Logic** (Logika Samar)
* **Evolutionary Algorithm** (Algoritma Evolusioner)
* **Swarm Intelligence** (Kecerdasan Kelompok)

---

## 🗺️ Roadmap Materi
Berikut adalah alur pembelajaran yang akan dibahas:
1. Fuzzy Logic
2. ANN (Artificial Neural Network)
3. Genetic Algorithm (Bagian dari Evolutionary Algorithm)
4. Particle Swarm Optimization / PSO (Bagian dari Swarm Intelligence)
5. Hybrid Model

---

## 📖 Detail Materi

### 1. Fuzzy Logic


Fuzzy Logic berfungsi untuk mendefinisikan suatu ketidakpastian menjadi hal yang terukur secara matematis (contohnya rentang batas antara "tinggi" dan "pendek").
* **Fungsi:** Menangani ketidakpastian (*uncertainty*) dan keaburan data.
* **Karakteristik Utama:** Menggunakan **derajat keanggotaan** (*degree of membership*) dengan nilai rentang antara 0 hingga 1.
* **Penerapan:** Sangat umum digunakan pada sistem kontrol (contoh: pengatur suhu AC, mesin cuci otomatis).

### 2. Neural Network


Sebuah sistem pemrosesan informasi yang arsitektur dan cara kerjanya terinspirasi dari jaringan saraf pada otak manusia.
* **Karakteristik Utama:** Mampu **belajar dari data** (*learning from data*).
* **Fungsi Utama:** Klasifikasi (*classification*) dan Prediksi (*prediction*).
> **Contoh Implementasi:** Computer Vision untuk menganalisa dan mengklasifikasikan ekspresi wajah manusia (sedih, senang, marah, netral).

### 3. Evolutionary Computation


Pendekatan optimasi yang terinspirasi dari teori seleksi alam dan genetika.
* **Siklus / Tahapan Utama:** Melibatkan konsep **Populasi**, **Seleksi**, **Crossover** (Persilangan), dan **Mutasi**.
* **Fungsi Utama:** Sangat baik digunakan untuk mencari nilai optimasi parameter pada ruang pencarian yang luas dan kompleks.

### 4. Swarm Intelligence


Metode komputasi yang terinspirasi dari perilaku sosial makhluk hidup yang hidup berkelompok. Sistem ini memecahkan masalah kompleks melalui interaksi individu-individu yang sederhana.
* **Contoh Algoritma:**
  * **Particle Swarm Optimization (PSO):** Terinspirasi dari pergerakan kawanan burung (*flock of birds*) atau ikan (*school of fish*).
  * **Ant Colony Optimization (ACO):** Terinspirasi dari perilaku koloni semut dalam menemukan jalur terpendek menuju sumber makanan.

### 5. Hybrid Model
Model Hybrid adalah pendekatan yang mengombinasikan dua atau lebih metode *Computational Intelligence* (CI).
* **Tujuan:** Untuk saling menutupi kelemahan tiap metode guna meningkatkan performa, stabilitas, atau akurasi sistem secara keseluruhan.

**Tabel Jenis Model Hybrid:**

| Jenis Hybrid | Konsep / Alur | Contoh Kombinasi |
| :--- | :--- | :--- |
| **Sequential Hybrid** | Output dari satu model menjadi input model lain <br> *(Input -> Model 1 -> Model 2 -> Output)* | **PSO -> ANN** (PSO digunakan untuk optimasi bobot ANN) |
| **Embedded Hybrid** | Satu metode melebur ke dalam proses metode lain <br> *(Input -> Proses Gabungan -> Output)* | **Neuro-Fuzzy** (ANFIS) |
| **Ensemble Hybrid** | Menggabungkan hasil prediksi dari beberapa model paralel | **Stacking** (Menggunakan *meta-learner*) |
| **Multi-stage Hybrid**| Proses yang melibatkan banyak tahap dan lebih dari dua model | **GA + ANN + Fuzzy** |