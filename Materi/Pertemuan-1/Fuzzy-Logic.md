### 1. Fuzzy Logic

Fuzzy Logic dipakai untuk memodelkan konsep yang tidak tegas seperti tinggi, rendah, panas, atau cukup pintar.
* **Fungsi:** menangani uncertainty dan keaburan data.
* **Karakteristik utama:** setiap nilai punya **derajat keanggotaan** antara 0 sampai 1.
* **Penerapan:** sistem kontrol seperti AC, mesin cuci, dan pengambilan keputusan sederhana.

#### Inti Konsep
Logika klasik memakai batas tegas, sedangkan fuzzy memberi ruang abu-abu.
* Himpunan crisp bersifat biner: 0 atau 1.
* Himpunan fuzzy memungkinkan satu nilai masuk ke beberapa kategori sekaligus dengan tingkat yang berbeda.

#### Komponen Utama
Materi pada buku menekankan tiga bagian besar:
* **Linguistic variable** untuk mewakili data dengan bahasa natural.
* **Membership function** untuk membentuk derajat keanggotaan.
* **Fuzzy rules** berbentuk IF-THEN untuk membuat keputusan.

#### Proses Inferensi Fuzzy
Alur dasarnya adalah:
1. **Fuzzification** mengubah nilai crisp menjadi nilai fuzzy.
2. **Inferencing** menghitung kekuatan aturan dengan operasi AND, OR, dan NOT.
3. **Defuzzification** mengubah hasil fuzzy menjadi nilai crisp.

#### Metode Inferensi
* **Mamdani**: consequent berupa himpunan fuzzy.
* **Sugeno**: consequent berupa konstanta atau fungsi.

#### Contoh Aplikasi
Contoh yang dipakai di materi adalah sistem beasiswa, dengan input seperti nilai dan pendapatan orang tua, lalu output berupa sedikit atau banyak beasiswa.