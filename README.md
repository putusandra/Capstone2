1. Pendahuluan

1.1 Latar Belakang

Customer Personality Analysis berikut ini adalah upaya perusahaan menggunakan data transaksi yang dikumpulkan selama dua tahun (antara 2012-2014) untuk melihat karakteristik pelanggan serta hubungannya terhadap perilaku belanja pelanggan pada masing-masing produk yang ditawarkan dan *campaign* yang dilakukan. Data disusun berdasarkan strategi *marketing* 4P: *People, Product, Promotion and Place.*

Hasil dari analisa ini diharapkan mampu memberi gambaran bagi  perusahaan mengenai kinerja *campaign* yang telah dilakukan. Serta memberi insight dalam menyusun perencanaan *marketing campaign* yang efektif dan efisien di masa depan. 


1.2 Rumusan Masalah

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

* ID: Id unik tiap customer
* Year_Birth: Tahun kelahiran
* Education: Tingkat pendidikan pelanggan
* Marital_Status: Status perkawinan pelanggan
* Income: Pendapatan pelanggan per tahun
* Kidhome: Jumlah kanak-kanak yang dimiliki pelanggan
* Teenhome: Jumlah anak remaja yang dimiliki pelanggan
* Dt_Customer: Tanggal pendaftaran pelanggan ke perusahaan
* Recency: Jumlah hari sejak pelanggan melakukan transaksi terakhir
* Complain: 1 jika pelanggan melakukan komplain sejak dua tahun terakhir, 0 lainnya

Products

* MntWines: nilai transaksi pembelian produk Wine selama dua tahun terakhir
* MntFruits: nilai transaksi pembelian produk Buah selama dua tahun terakhir
* MntMeatProducts: nilai transaksi pembelian daging selama dua tahun terakhir
* MntFishProducts: nilai transaksi pembelian Ikan selama dua tahun terakhir
* MntSweetProducts: nilai transaksi pembelian Manisan selama dua tahun terakhir
* MntGoldProds: nilai transaksi pembelian Emas selama dua tahun terakhir

Promotion

* NumDealsPurchases: Jumlah pembelian menggunakan diskon
* AcceptedCmp1: 1 jika pelanggan menerima penawaran di kampanye pemasaran ke-1, 0 lainnya
* AcceptedCmp2: 1 jika pelanggan menerima penawaran di kampanye pemasaran ke-2, 0 lainnya
* AcceptedCmp3: 1 jika pelanggan menerima penawaran di kampanye pemasaran ke-3, 0 lainnya
* AcceptedCmp4: 1 jika pelanggan menerima penawaran di kampanye pemasaran ke-4, 0 lainnya
* AcceptedCmp5: 1 jika pelanggan menerima penawaran di kampanye  pemasaran ke-5, 0 lainnya
* Response: 1 jika pelanggan menerima penawaran di kampanye pemasaran yang terakhir, 0 lainnya

Place

* NumWebPurchases: Jumlah pembelian melalui website perusahaan
* NumCatalogPurchases: Jumlah pembelian melalui katalog
* NumStorePurchases: Jumlah pembelian langsung di toko
* NumWebVisitsMonth: Jumlah kunjungan ke website perusahaan pada bulan terakhir

Other

* Z_CostContact: Kolom tidak mempunyai arti pada dataset dan tidak mempunyai peran dalam analisis.
* Z_Revenue: Kolom tidak mempunyai arti pada dataset dan tidak mempunyai peran dalam analisis.
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
