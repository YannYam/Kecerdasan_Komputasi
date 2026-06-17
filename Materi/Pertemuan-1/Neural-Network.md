### 2. Neural Network

Neural Network atau Jaringan Syaraf Tiruan adalah sistem pemrosesan informasi yang terinspirasi dari cara kerja saraf manusia.
* **Karakteristik utama:** belajar dari data.
* **Fungsi utama:** klasifikasi dan prediksi.
* **Contoh implementasi:** computer vision, pengenalan wajah, dan analisis data medis.

#### Perceptron
Perceptron adalah bentuk JST paling sederhana, memakai satu layer output untuk klasifikasi biner.
* Data latih berisi pasangan input dan target output.
* Bobot dan bias diperbarui saat output salah.
* Cocok untuk data yang **linearly separable**.

#### Supervised Learning
Pada supervised learning, model dilatih memakai data input-target untuk mencari bobot dan bias terbaik.
* Pembelajaran dilakukan sampai jumlah epoch tertentu atau error minimum tercapai.
* Gradient descent dipakai untuk menurunkan error.
* Update bisa dilakukan secara online, stochastic, atau batch.

#### Multi Layer Perceptron
MLP menambahkan hidden layer sehingga bisa menyelesaikan masalah yang tidak bisa ditangani perceptron tunggal.
* Terdiri dari input layer, hidden layer, dan output layer.
* Menggunakan feedforward untuk menghitung output.
* Menggunakan backpropagation untuk memperbaiki bobot berdasarkan error.

#### Inti Kesimpulan
Jika data tidak bisa dipisahkan secara linear, jaringan dengan lebih dari satu layer diperlukan. Contoh klasiknya adalah masalah XOR.