# Praktikum-Dimensionality-Reduction-PCA-t-SNE-NayHana

# Dimensionality Reduction pada Data Mobile Game In-App Purchases

Repository ini berisi tugas praktikum implementasi metode dimensionality reduction, yaitu PCA dan t-SNE, menggunakan dataset pembelian dalam aplikasi mobile game.

## Deskripsi Kasus
Dataset Mobile Game In-App Purchases memiliki banyak fitur numerik yang merepresentasikan perilaku pemain, seperti umur, jumlah sesi bermain, durasi sesi, dan total pembelian. Dengan jumlah dimensi yang cukup tinggi, visualisasi langsung terhadap data menjadi sulit dan pola perilaku pemain tidak mudah diidentifikasi.

Oleh karena itu, dimensionality reduction digunakan untuk merangkum informasi penting dari data berdimensi tinggi ke dalam ruang berdimensi rendah (2D), sehingga pola pengelompokan pemain berdasarkan segmentasi ekonomi (*Whale*, *Dolphin*, dan *Minnow*) dapat diamati secara visual.

## Dataset
Dataset yang digunakan adalah **Mobile Game In-App Purchases Dataset 2025** yang berisi:
- **Fitur numerik**: `Age`, `SessionCount`, `AverageSessionLength`, `InAppPurchaseAmount`, dan fitur numerik lainnya.
- **Label/target**: `SpendingSegment`.

## Metode
1. **StandardScaler**  
   Digunakan untuk menormalkan data agar setiap fitur memiliki skala yang sebanding sebelum proses reduksi dimensi.

2. **PCA (Principal Component Analysis)**  
   Digunakan untuk mereduksi dimensi secara linier dengan mempertahankan variasi data terbesar, sehingga dapat memberikan gambaran global struktur data.

3. **t-SNE (t-Distributed Stochastic Neighbor Embedding)**  
   Digunakan untuk visualisasi non-linier yang berfokus pada pelestarian struktur lokal, sehingga cocok untuk eksplorasi pola dan klaster perilaku pemain.

## Analisis Hasil
Hasil visualisasi menggunakan PCA menunjukkan distribusi global data pemain berdasarkan variasi terbesar, namun pemisahan antar segmen belanja masih terlihat tumpang tindih karena sifat PCA yang linier.

Sebaliknya, visualisasi menggunakan t-SNE mampu menampilkan pengelompokan pemain dengan lebih jelas. Beberapa segmen belanja membentuk klaster yang relatif terpisah, menunjukkan adanya kemiripan pola perilaku dan pengeluaran di dalam masing-masing kelompok.

Berdasarkan hasil tersebut, t-SNE dinilai lebih sesuai untuk keperluan eksplorasi klaster perilaku pemain pada dataset ini, sedangkan PCA tetap bermanfaat sebagai tahap awal reduksi dimensi dan pemahaman struktur data secara umum.

## Anggota Kelompok
- Nayla Raihaanah Nabilah Hakim (24523010)
- Raihana Salwa Hafizhah (24523072)
