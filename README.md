# Supermarket Sales Analysis

Portfolio project analisis penjualan dan prediksi keuntungan pada data supermarket Indonesia periode 2014–2017. Proyek ini dibuat sebagai bagian dari pembelajaran **Belajar Analisis Data untuk Pemula** pada Learning Path Data Analyst Dicoding.

## Ringkasan Proyek

Proyek ini mengolah data transaksi supermarket untuk menghasilkan dashboard informasi penjualan dan membangun model prediksi keuntungan. Analisis dilakukan menggunakan spreadsheet dan Looker Studio, sedangkan pemodelan prediktif dibuat melalui Orange Data Mining.

## Tujuan Analisis

- Mengidentifikasi tren penjualan selama periode 2014–2017.
- Membandingkan jumlah pesanan berdasarkan wilayah.
- Menganalisis kontribusi penjualan setiap kategori produk.
- Menentukan kota, bulan, dan metode pengiriman yang paling menonjol.
- Membandingkan model Linear Regression dan Random Forest untuk memprediksi keuntungan.

## Dataset

Dataset sintetis berisi **10.076 baris transaksi** dengan cakupan tahun 2014–2017. Beberapa atribut utama yang digunakan meliputi:

- Tanggal pemesanan dan pengiriman
- Metode pengiriman
- Segmen pelanggan
- Kota dan wilayah
- Kategori dan subkategori produk
- Penjualan, kuantitas, diskon, dan keuntungan

> Dataset pada proyek ini bersifat sintetis dan digunakan untuk keperluan pembelajaran serta demonstrasi portofolio.

## Proses Analisis

1. Memeriksa struktur, tipe data, nilai kosong, dan konsistensi data.
2. Membersihkan tanggal pengiriman, kota, dan kode pos.
3. Melakukan analisis deskriptif terhadap penjualan dan pesanan.
4. Membuat visualisasi interaktif menggunakan Looker Studio.
5. Menentukan `keuntungan` sebagai target prediksi.
6. Menggunakan penjualan, kuantitas, diskon, metode pengiriman, segmen, kota, kategori, dan subkategori sebagai fitur.
7. Membandingkan Linear Regression dan Random Forest menggunakan 5-fold cross-validation.

## Insight Utama

Berdasarkan dashboard yang dibuat:

- Tren penjualan berfluktuasi setiap bulan, tetapi secara umum meningkat selama 2014–2017.
- Wilayah Central mempunyai proporsi jumlah pesanan terbesar, sekitar 38,4%.
- Kategori Technology memberikan kontribusi penjualan terbesar, sekitar 36,3%.
- Balikpapan tercatat sebagai kota dengan total penjualan tertinggi.
- Standard Class menjadi metode pengiriman yang paling sering digunakan.
- November menjadi bulan dengan total penjualan tertinggi selama periode analisis.

## Analisis Prediktif

Dua algoritma regresi dibandingkan:

- Linear Regression
- Random Forest

Pada evaluasi proyek, Random Forest menghasilkan nilai R² sekitar **0,746**, lebih tinggi daripada Linear Regression. Hasil tersebut menunjukkan bahwa Random Forest menjadi model yang lebih baik pada eksperimen ini dalam menjelaskan variasi nilai keuntungan.

## Dashboard

- [Buka dashboard Looker Studio](https://datastudio.google.com/reporting/69a5f62f-95ca-44d8-8202-c61b0c4c4f82)
- [Buka data pada Google Sheets](https://docs.google.com/spreadsheets/d/1Jc5dlAdH573pEsI3SWK8MQeS_925Kjb09yvB5cotXjQ/edit?usp=sharing)
- Versi PDF dashboard tersedia di folder `dashboard/`.

## Struktur Repository

```text
supermarket-sales-analysis/
├── README.md
├── data/
│   └── synthetic_store_indonesia.xlsx
├── dashboard/
│   └── informasi_penjualan_supermarket_indonesia.pdf
├── model/
│   └── analisis-prediktif-supermarket.ows
└── links/
    └── url.txt
```

## Cara Membuka Proyek

### Dashboard

Buka tautan Looker Studio pada bagian Dashboard atau unduh file PDF pada folder `dashboard`.

### Model Orange

1. Instal [Orange Data Mining](https://orangedatamining.com/).
2. Unduh dataset pada folder `data`.
3. Unduh file `.ows` pada folder `model`.
4. Buka file workflow menggunakan Orange.
5. Apabila sumber data tidak ditemukan otomatis, arahkan widget File ke dataset yang telah diunduh.

## Tools

- Microsoft Excel / Spreadsheet
- Google Sheets
- Looker Studio
- Orange Data Mining
- Linear Regression
- Random Forest

## Author

**Muhammad Reza Pahlevi Harahap**

- GitHub: [RezaHarahap](https://github.com/RezaHarahap)
- Dicoding: [reza_harahap](https://www.dicoding.com/users/reza_harahap)

## Catatan

Proyek ini dibuat untuk tujuan pembelajaran dan portofolio. Insight serta hasil prediksi tidak ditujukan sebagai rekomendasi bisnis pada kondisi nyata tanpa validasi lanjutan.
