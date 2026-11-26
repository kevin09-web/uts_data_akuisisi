Berikut README yang bisa kamu gunakan untuk proyek UTS Data Acquisition & Management. Saya susun berdasarkan tiga metode akuisisi yang sudah kamu kerjakan: Kaggle, API Open-Meteo, dan web scraping Wikipedia.

Kamu bisa membuat file baru bernama `README.md` di folder utama proyek Google Colab atau GitHub.

# UTS DATA ACQUISITION & MANAGEMENT

## Akuisisi Data Pariwisata Indonesia

### 1. Identitas Mahasiswa

| Keterangan    | Informasi                      |
| ------------- | ------------------------------ |
| Nama          | I Nyoman Cahyanta Kusumadinata |
| NIM           | 2501010166                     |
| Program Studi | Informatika                    |
| Kelas         | F                              |
| Mata Kuliah   | Data Acquisition & Management  |
| Semester      | Ganjil                         |
| Tahun         | 2026                           |

### 2. Deskripsi Proyek

Proyek ini merupakan tugas Ujian Tengah Semester (UTS) mata kuliah Data Acquisition & Management yang berfokus pada proses pengumpulan, pengolahan, dan penggabungan data dengan tema pariwisata Indonesia.

Pengumpulan data dilakukan menggunakan tiga metode, yaitu mengunduh dataset dari Kaggle, mengambil data melalui API Open-Meteo, dan melakukan web scraping pada halaman Wikipedia. Data yang diperoleh kemudian diperiksa, dibersihkan, diolah, serta digabungkan untuk menghasilkan informasi yang berkaitan dengan destinasi wisata dan kondisi cuaca di beberapa kota di Indonesia.

### 3. Goal (Tujuan Utama)

Membangun kumpulan data pariwisata Indonesia yang menggabungkan informasi destinasi wisata dengan kondisi cuaca berdasarkan wilayah kota, sehingga menghasilkan data yang lebih informatif dan dapat digunakan untuk analisis sederhana.

### 4. Tujuan Proyek

1. Memahami dan menerapkan tiga metode akuisisi data, yaitu dataset terbuka, API, dan web scraping.
2. Mengumpulkan informasi destinasi wisata di Indonesia dari sumber dataset Kaggle.
3. Mengambil informasi cuaca berdasarkan kota melalui API Open-Meteo.
4. Mengumpulkan informasi warisan dunia Indonesia melalui web scraping.
5. Melakukan pemeriksaan kualitas, pembersihan, dan identifikasi karakteristik data.
6. Menerapkan penggabungan data menggunakan fungsi `merge()` dengan kunci penggabungan yang sesuai.
7. Menghasilkan dataset gabungan yang dapat digunakan sebagai dasar analisis pariwisata.

### 5. Sumber Data dan URL

| No. | Metode Akuisisi | Sumber Data                                           | URL                                                                                                                                                |
| --- | --------------- | ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Dataset Terbuka | Kaggle - Indonesia Tourism Destination                | [https://www.kaggle.com/datasets/aprabowo/indonesia-tourism-destination](https://www.kaggle.com/datasets/aprabowo/indonesia-tourism-destination)   |
| 2   | API             | Open-Meteo Historical Weather API                     | [https://archive-api.open-meteo.com/v1/archive](https://archive-api.open-meteo.com/v1/archive)                                                     |
| 3   | Web Scraping    | Wikipedia - List of World Heritage Sites in Indonesia | [https://en.wikipedia.org/wiki/List_of_World_Heritage_Sites_in_Indonesia](https://en.wikipedia.org/wiki/List_of_World_Heritage_Sites_in_Indonesia) |

### 6. Informasi Data yang Dikumpulkan

**A. Dataset Kaggle**

- Data destinasi wisata Indonesia.
- Informasi nama tempat wisata.
- Kategori wisata.
- Kota lokasi wisata.
- Harga tiket dan rating destinasi.
- Koordinat geografis.

**B. API Open-Meteo**

- Suhu rata-rata harian.
- Suhu maksimum dan minimum.
- Curah hujan.
- Kecepatan angin maksimum.
- Tanggal dan lokasi pengamatan.

Wilayah pengamatan meliputi Bandung, Jakarta, Semarang, Surabaya, dan Yogyakarta dengan periode 1–30 Januari 2025.

**C. Web Scraping Wikipedia**

- Informasi daftar situs warisan dunia di Indonesia.
- Nama situs.
- Tahun penetapan dan informasi lain sesuai tabel sumber.

### 7. Hasil Pengolahan Data

Data dari ketiga metode akuisisi diproses dan disimpan secara terpisah. Dataset pariwisata dan data cuaca kemudian digabungkan berdasarkan nama kota.

Hasil penggabungan menghasilkan informasi destinasi wisata yang dilengkapi dengan ringkasan kondisi cuaca berdasarkan kota masing-masing.

### 8. Struktur Folder Proyek

```
UTS-DAM-Pariwisata/
│── Dam_Pariwisata.ipynb
├── README.md
├── DATA ETHICS CHECKLIST.dock
│
└── data/
    ├── raw/
    │   ├── kaggle/
    │   ├── api/
    │   └── scraping/
    │
    └── processed/
        ├── tourism_cleaned.csv
        ├── data_cuaca_pariwisata.csv
        ├── data_warisan_dunia_indonesia.csv
        ├── data_gabungan_pariwisata_cuaca.csv
        └── metadata_penggabungan.json
```

### 9. Tools dan Library

- Python
- Google Colab
- Pandas
- Requests
- BeautifulSoup
- JSON
- Hashlib

### 10. Kesimpulan

Melalui proyek ini, dilakukan penerapan tiga metode akuisisi data dalam satu tema, yaitu pariwisata Indonesia. Setiap sumber memiliki karakteristik dan bentuk data yang berbeda. Setelah melalui proses pengolahan, data destinasi wisata dan cuaca dapat digabungkan berdasarkan wilayah kota untuk menghasilkan informasi yang lebih lengkap.

Proyek ini memberikan pemahaman mengenai proses akuisisi data, pemeriksaan kualitas, etika penggunaan data, provenance, web scraping, API, serta penggabungan dataset menggunakan Python.

Catatan: URL tabel Wikipedia di atas adalah halaman sumber scraping, sedangkan URL API adalah endpoint dasar. README ini merupakan dokumentasi proyek, bukan pengganti catatan provenance yang memuat tanggal akses, lisensi, dan hash MD5.
