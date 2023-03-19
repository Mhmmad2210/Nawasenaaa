
# EDA - Stage 1

## Data Set Sample

Dataset ini merupakan Dataset yang terdiri dari 18 fitur dan 12.330 baris
dataset ini berisikan data dari waktu setiap pengguna dan aplikasi apa yang digunakan untuk membuka e-commerce.

Download data set [Here](https://www.kaggle.com/datasets/imakash3011/online-shoppers-purchasing-intention-dataset)



## Descriptive Statistics
Gunakan function info dan describe pada dataset final project kalian. Tuliskan hasil observasinya, seperti:

A. Apakah ada kolom dengan tipe data kurang sesuai, atau nama kolom dan isinya kurang sesuai?

penggunaan `df.info()` untuk melihat tipe data dari setiap fitur dan jumlah baris


B. Apakah ada kolom yang memiliki nilai kosong? Jika ada, apa saja?

penggunaan `df.isna()` untuk melihat apakah setiap fitur memiliki nilai kosong atau tidak.

C. Apakah ada kolom yang memiliki nilai summary agak aneh?
(min/mean/median/max/unique/top/freq)

dilakukan pengkategorian pada setiap fitur dan dijadikan 2 jenis kategori `num` dan `cats`. kemudian menggunakan `describe` untuk mendapatkan (min/mean/median/max/unique/top/freq)

## Univariate Analysis

Gunakan visualisasi untuk melihat distribusi masing-masing kolom (feature maupun target). Tuliskan hasil observasinya, misalnya jika ada suatu kolom yang distribusinya menarik (misal skewed, bimodal, ada outlier, ada nilai yang mendominasi, kategorinya terlalu banyak, dsb). Jelaskan juga apa yang harus di-follow up saat data pre-processing. Diawali dengan Menghilangkan outlier!

pengecekan distribusi pada data numerical menggunakan grafik `boxplot` dan `kdplot`

pengecekan distribusi pada data kategorical menggunakan grafik `countplot`

## Multivariate Analysis 
Lakukan multivariate analysis (seperti correlation heatmap dan category plots, sesuai yang diajarkan di kelas). Tuliskan hasil observasinya, seperti:

A. Bagaimana korelasi antara masing-masing feature dan label. Kira-kira feature mana saja yang paling relevan dan harus dipertahankan?

digunakan grafik `pairplot` untuk meihat korelasi berbagai fitur lain terhadap fitur revenue

B. Bagaimana korelasi antar-feature, apakah ada pola yang menarik? Apa yang perlu dilakukan terhadap feature itu?

korelasi antar fitur bisa dilihat dengan menggunakan grafik `heatmap`.

korelasi antara fitur numerical dan kategorical bisa dilihat menggunakan grafik `barplot` 

### Hasil korelasi

Page Values memiliki korelasi paling kuat terhadap Revenue, sedangkan Administrative, ProductRelated, dan ProductRelated_Duration cukup kuat terhadap Revenue BounceRates, ExitRates memiliki korelasi negatif yang cukup kuat terhadap Revenue Beberapa fitur cukup baik digunakan seperti PageValues, ProductRelated, ProductRelated_Duration, Administrative, BounceRates, dan ExitRates Sedangkan feature yang lain kurang memiliki korelasi terhadap Revenue

## Business Insight 

Selain EDA, lakukan juga beberapa analisis dan visualisasi untuk menemukan suatu business insight. Tuliskan minimal 3 insight, dan berdasarkan insight tersebut jelaskan rekomendasinya untuk bisnis. Insight

* Jumlah visit terbanyak terdapat pada Region 1, sehingga untuk  meningkatkan tingkat ketertarikan pengunjung website e-commerce dari Region lain dapat dilakukan promosi misalnya gratis biaya pengiriman (Ongkir).

* Pada Kolom Month didapatkan informasi bahwa pada bulan Desember, Maret, Mei dan November merupakan bulat yang paling sering didatangi oleh pengunjung. Sebagai solusi bisa diadakan event di setiap bulan misalnya 1.1 (1 Januari) atau 2.2 (2 Februari) dan seterusnya agar di bulan lainnya juga mengalami kenaikan jumlah pengunjung.

* Tipe Visitor terbanyak merupakan Returning Visitor, sehingga kita dapat memberikan kupon potongan harga pada saat belanja berikutnya agar tipe pelanggan ini merasa senang. Sedangkan untuk tipe New Visitor dapat kita berikan produk gratis dengan syarat melakukan transaksi senilai yang ditentukan terlebih dahulu.

* Pengunjung website e-commerce pada saat weekday lebih banyak dari pada saat weekend, sehingga kita dapat memberikan promo atau event yang menarik pada saat weekend untuk menarik atensi pelanggan.
