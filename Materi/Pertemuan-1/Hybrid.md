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