### 2. Swarm Intelligence

Swarm Intelligence adalah algoritma berbasis populasi yang meniru perilaku kolektif organisme sosial seperti burung, ikan, dan semut.
* **Fungsi:** menyelesaikan optimasi non-linear dan pencarian ruang solusi yang kompleks.
* **Karakteristik utama:** terdesentralisasi, dan solusi global muncul dari aturan lokal sederhana.
* **Penerapan:** penjadwalan, optimasi rute, optimasi fungsi matematika, dan pelatihan JST.

#### A. Particle Swarm Optimization (PSO)
PSO terinspirasi dari kawanan burung yang mencari makanan.
* Setiap kandidat solusi disebut partikel.
* Partikel menyimpan **pbest** dan dipandu oleh **gbest**.
* Posisi dan kecepatan diperbarui secara iteratif sampai solusi membaik.

PSO cocok untuk ruang pencarian kontinu seperti optimasi parameter dan fungsi numerik.

#### B. Ant Colony Optimization (ACO)
ACO terinspirasi dari koloni semut yang menemukan rute terpendek ke sumber makanan.
* Jalur yang sering dilewati akan memiliki pheromone lebih pekat.
* Semut berikutnya memilih jalur berdasarkan probabilitas dan informasi heuristik jarak.
* Pheromone menguap seiring waktu agar algoritma tidak cepat terjebak pada solusi lokal.

ACO lebih cocok untuk masalah diskrit atau kombinatorial seperti graph dan travelling salesman problem.

#### Inti Perbandingan
* **PSO** kuat untuk ruang kontinu dengan komunikasi langsung antar partikel.
* **ACO** kuat untuk ruang diskrit dengan komunikasi tidak langsung melalui jejak pheromone.