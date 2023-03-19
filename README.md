
1. Descriptive Statistics

A. Apakah ada kolom dengan tipe data kurang sesuai, atau nama kolom dan isinya 
kurang sesuai

Setelah di periksa semua tipe data sudah sesuai yang diperlukan

B. Apakah ada kolom yang memiliki nilai kosong? Jika ada, apa saja?

Tidak ada data yang kosong 

C. Apakah ada kolom yang memiliki nilai summary agak aneh?
Banyak kolom yang memiliki perbedaan yang sangat signifikan pada nilai mean dan median.
Nilai unique dan freq cenderung normal, tidak terlalu timpang

2.Univariate Analysis
Gunakan visualisasi untuk melihat distribusi masing-masing kolom (feature maupun target). Tuliskan hasil observasinya, misalnya jika ada suatu kolom yang distribusinya menarik (misal skewed, bimodal, ada outlier, ada nilai yang mendominasi, kategorinya terlalu banyak, dsb). Jelaskan juga apa yang harus di-follow up saat data pre-processing.
Diawali dengan Menghilangkan outlier!

Multivariate Analysis
Lakukan multivariate analysis (seperti correlation heatmap dan category plots, sesuai yang diajarkan di kelas). Tuliskan hasil observasinya, seperti:

A. Bagaimana korelasi antara masing-masing feature dan label. Kira-kira feature mana saja yang paling relevan dan harus dipertahankan?

B. Bagaimana korelasi antar-feature, apakah ada pola yang menarik? Apa yang perlu dilakukan terhadap feature itu?

Tuliskan juga jika memang tidak ada feature yang saling berkorelasi

Page Values memiliki korelasi paling kuat terhadap Revenue, sedangkan Administrative, ProductRelated, dan ProductRelated_Duration cukup kuat terhadap Revenue
BounceRates, ExitRates memiliki korelasi negatif yang cukup kuat terhadap Revenue
Beberapa fitur cukup baik digunakan seperti PageValues, ProductRelated, ProductRelated_Duration, Administrative, BounceRates, dan ExitRates
Sedangkan feature yang lain kurang memiliki korelasi terhadap Revenue

Business Insight
Selain EDA, lakukan juga beberapa analisis dan visualisasi untuk menemukan suatu business insight. Tuliskan minimal 3 insight, dan berdasarkan insight tersebut jelaskan rekomendasinya untuk bisnis.
Insight

Jumlah visit terbanyak terdapat pada Region 1, sehingga untuk meningkatkan tingkat ketertarikan pengunjung website e-commerce dari Region lain dapat dilakukan promosi misalnya gratis biaya pengiriman (Ongkir).

Pada Kolom Month didapatkan informasi bahwa pada bulan Desember, Maret, Mei dan November merupakan bulat yang paling sering didatangi oleh pengunjung. Sebagai solusi bisa diadakan event di setiap bulan misalnya 1.1 (1 Januari) atau 2.2 (2 Februari) dan seterusnya agar di bulan lainnya juga mengalami kenaikan jumlah pengunjung.

Tipe Visitor terbanyak merupakan Returning Visitor, sehingga kita dapat memberikan kupon potongan harga pada saat belanja berikutnya agar tipe pelanggan ini merasa senang. Sedangkan untuk tipe New Visitor dapat kita berikan produk gratis dengan syarat melakukan transaksi senilai yang ditentukan terlebih dahulu.

Pengunjung website e-commerce pada saat weekday lebih banyak dari pada saat weekend, sehingga kita dapat memberikan promo atau event yang menarik pada saat weekend untuk menarik atensi pelanggan.
