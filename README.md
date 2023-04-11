#**1. Pendahuluan**

###**1.1 Latar Belakang**

*Customer Personality Analysis* berikut ini adalah upaya perusahaan menggunakan data transaksi yang dikumpulkan selama dua tahun (antara 2012-2014) untuk melihat karakteristik pelanggan serta hubungannya terhadap perilaku belanja pelanggan pada masing-masing produk yang ditawarkan dan *campaign* yang dilakukan. Data disusun berdasarkan strategi *marketing* 4P: *People, Product, Promotion and Place.*

Hasil dari analisa ini diharapkan mampu memberi gambaran bagi  perusahaan mengenai kinerja *campaign* yang telah dilakukan. Serta memberi insight dalam menyusun perencanaan *marketing campaign* yang efektif dan efisien di masa depan. 


###**1.2 Rumusan Masalah**

Perusahaan ingin memaksimalkan *marketing campaign* produk agar tepat sasaran sesuai kelompok pelanggan yang berpeluang besar untuk melakukan transaksi. Selain itu, menerapkan strategi diskon dan beriklan melalui platform/pendekatan yang paling efektif berdasarkan demografi pelanggan. Baik melalui online maupun offline marketing. Data analyst membuat usulan berdasarkan pertanyaan berikut:

1. Bagaimana karakteristik pelanggan secara umum dalam dua tahun terakhir?
2. Bagaimana gambaran segmen pelanggan yang memiliki pendapatan tertinggi? Adakah hubungan antara kelas pendapatan dengan total pengeluaran?
3. Bagaimana gambaran segmen pelanggan yang melakukan transaksi lebih banyak?
4. Apa jenis produk dengan penjualan tertinggi dalam dua tahun terakhir? Seperti apa segmen pelanggan yang terbanyak membeli produk tersebut?
5. Bagaimana hubungan antara status pernikahan, jumlah anak, serta pengeluaran?
6. Bagaimana proporsi penjualan di masing-masing lini penawaran (web, store, catalog)? 
7. Berapa persen campaign direspon oleh pelanggan dan terkonversi menjadi transaksi? Segmen pelanggan seperti apa yang paling banyak merespon?
8. Bagaimana hubungan antara lini penawaran produk dengan kelompok usia dan tingkat pendidikan? 
9. Berapa persen jumlah kunjangan website terkonversi menjadi transaksi?
10. Bagaimana hubungan antara total pengeluaran dan total kampanye yang direspon pelanggan? 
11. Bagaimana gambaran segmen pelanggan yang terbanyak bertransaksi dengan diskon?
12. Bagaimana gambaran pertumbuhan pelanggan baru selama 2 tahun terakhir?
13. Bagaimana kita memperoleh informasi mengenai value dan loyalitas setiap pelanggan terhadap perusahaan?


People
ID: ID unik customer
Year_Birth: Tahun lahir customer
Education: Level pendidikan customer
Marital_Status: Status pernikahan customer
Income: Pendapatan rumah tangga tahunan customer
Kidhome: Jumlah anak kecil yang dimiliki customer
Teenhome: Jumlah remaja yang dimiliki customer
Dt_Customer: Tanggal pendaftaran customer ke perusahaan
Recency: Jumlah hari sejak customer melakukan pembelian terakhir
Complain: 1 jika customer complain dalam 2 tahun terakhir, 0 sebaliknya

Products
MntWines: Jumlah yang dibelanjakan untuk Wine dalam 2 tahun terakhir
MntFruits: Jumlah yang dibelanjakan untuk Buah dalam 2 tahun terakhir
MntMeatProducts: Jumlah yang dibelanjakan untuk Daging dalam 2 tahun terakhir
MntFishProducts: Jumlah yang dibelanjakan untuk Ikan dalam 2 tahun terakhir
MntSweetProducts: Jumlah yang dibelanjakan untuk produk Makanan Manis dalam 2 tahun terakhir
MntGoldProds: Jumlah yang dibelanjakan untuk Emas dalam 2 tahun terakhir

Promotion
NumDealsPurchases: Jumlah pembelian yang menggunakan diskon
AcceptedCmp1: 1 jika customer menerima penawaran dari campaign ke-1, 0 sebaliknya
AcceptedCmp2: 1 jika customer menerima penawaran dari campaign ke-2, 0 sebaliknya
AcceptedCmp3: 1 jika customer menerima penawaran dari campaign ke-3, 0 sebaliknya
AcceptedCmp4: 1 jika customer menerima penawaran dari campaign ke-4, 0 sebaliknya
AcceptedCmp5: 1 jika customer menerima penawaran dari campaign ke-5, 0 sebaliknya
Response: 1 jika customer menerima penawaran dari campaign terakhir, 0 sebaliknya

Place
NumWebPurchases: Jumlah pembelian yang dilakukan melalui website perusahaan
NumCatalogPurchases: Jumlah pembelian yang dilakukan menggunakan katalog
NumStorePurchases: Jumlah pembelian yang dilakukan langsung di toko
NumWebVisitsMonth: Jumlah kunjungan ke website perusahaan dalam sebulan terakhir

Others
Z_CostContact: Kolom irrelevan dengan dataset "Customer Personality Analysis"
Z_Revenue: Kolom irrelevan dengan dataset "Customer Personality Analysis"

Data Wrangling
Handling missing values
Drop irrelevant columns
Checking outliers

Dalam analisis data, rumusan masalah akan dijabarkan ke dalam poin-poin berikut ini: 

3.1 Karakteristik Pelanggan
* Kelompok usia pelanggan
* Background pendidikan pelanggan
* Parental Status dan Marital Status
* Jumlah anak pelanggan
* Distribusi usia pelanggan
* Distribusi total pengeluaran
* Distribusi income pelanggan

3.2 Korelasi
* Matriks korelasi sebagai gambaran umum
* Hubungan antara segmen usia dengan income
* Hubungan antara segmen usia, income, dan total pengeluaran
* Hubungan parental status dengan income dan total pengeluaran
* Hubungan antara total pengeluaran, income, dan jumlah anak

3.3 Marketing Campaign Analysis
* proporsi banyaknya transaksi produk berdasarkan masing-masing lini penawaran 
* Hubungan segmen pendidikan dengan lini penawaran dan campaign yang diterima
* Respon pelanggan terhadap marketing campaign yang telah dilakukan
* Gambaran pertumbuhan pelanggan berdasarkan bulan
* Melihat value dari setiap pelanggan untuk personalisasi target penawaran
