# Dekoruma_Analysis
# Tentang Dekoruma
Dekoruma adalah perusahaan e-commerce furnitur dan dekorasi rumah asal Indonesia. Dekoruma menjual produk melalui tiga channel: toko fisik (DEC), website, dan mobile app. Salah satu keunggulan Dekoruma adalah layanan perakitan (Installation Service) yang menjadi nilai tambah utama bagi pelanggan yang membeli furniture di Dekoruma.

# Masalah
Tingginya biaya operasional retur dan anjloknya kepuasan pelanggan akibat jadwal pengiriman dan perakitan furnitur (Bulky Goods) yang tidak sinkron, banyaknya komponen cacat/hilang, serta adanya dugaan showrooming untuk beberapa toko fisik. Showrooming adalah kejadian dimana pelanggan tinggal dekat salah satu toko fisik, tetapi memesan melalui aplikasi/website.

# Data yang digunakan
Analisis menggunakan data dari tiga tabel format csv, yaitu:
- dekoruma_orders.csv = Data transaksi utama, mengandung 300.000 baris 9 kolom, dimana 1 baris adalah 1 transaksi/order
- dekoruma_products.csv = Data produk, mengandung 1.500 baris 4 kolom, setiap baris adalah 1 SKU/produk
- dekoruma_stores.csv = Data toko/channel type, mengandung 40 baris 3 kolom, 38 baris merupakan toko fisik dan 2 lain nya adalah aplikasi (app) dan website  
Setelah dilakukan data cleansing, masing-masing tabel disimpan sebagai:
- dekoruma_orders_clean.csv
- dekoruma_products_clean.csv
- dekoruma_stores_clean.csv

# Analisis
Untuk menjawab masalah yang dijelaskan sebelumnya, maka dilakukan 4 analisis, yaitu tentang:
- Rentang hari kedatangan tukang rakit dari tanggal barang tiba
- Kasus kegagalan perakitan dan rasio kegagalan nya (failure rate %)
- Kasus kekurangan komponen oleh toko, dan bagaimana persebaran nya
- Transaksi kejadian showrooming dengan melihat selisih/rentang waktu dari pelanggan bayar ke tanggal barang tiba (delivered).
