# 5. Algoritma Genetika (Genetic Algorithm)

Algoritma Genetika adalah teknik optimasi yang meniru evolusi biologis untuk mencari solusi terbaik.
* **Tujuan:** mendapatkan solusi optimal dari banyak kemungkinan solusi.
* **Ide utama:** setiap kandidat solusi direpresentasikan sebagai kromosom yang terdiri dari gen.
* **Contoh masalah:** fungsi optimasi, travelling salesman problem, dan feature selection.

## A. Komponen Utama
Sebelum AG dijalankan, dua hal harus disiapkan:
1. **Representasi individu / kromosom** sebagai kandidat solusi.
2. **Fungsi fitness** untuk mengukur kualitas solusi.

Pada TSP, fitness sering dihitung sebagai kebalikan dari jarak karena tujuan utamanya adalah mencari rute terpendek.

## B. Operasi Genetika
Proses AG dilakukan berulang pada setiap generasi:
1. **Inisialisasi** populasi awal.
2. **Seleksi** parent berdasarkan fitness, misalnya dengan roulette wheel atau rank-based selection.
3. **Crossover** untuk menukar gen dan membentuk offspring baru.
4. **Mutasi** untuk menjaga variasi dan menghindari solusi lokal.

## C. Elitism
Elitism mempertahankan individu terbaik agar tidak hilang di generasi berikutnya.
* Menjaga solusi terbaik tetap ada selama proses evolusi.
* Membuat konvergensi lebih stabil.

## D. Inti Penerapan
AG cocok dipakai untuk masalah pencarian rute, penjadwalan, dan pemilihan fitur karena mampu menjelajah ruang solusi yang besar tanpa harus mencari secara eksak.