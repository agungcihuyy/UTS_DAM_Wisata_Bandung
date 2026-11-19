# UTS Data Acquisition and Management
## Analisis Objek Wisata Belanja di Kota Bandung

### 1. Data Diri

| Keterangan | Identitas |
|---|---|
| Nama | I Gusti Lanang Agung Wahyu Pandu Rangga |
| NIM | 2501010026 |
| Program Studi | Informatika |
| Perguruan Tinggi | INSTIKI |
| Kelas | E |
| Mata Kuliah | Data Acquisition and Management |
| Tugas | Ujian Tengah Semester (UTS) |

### 2. Deskripsi Proyek

Proyek ini dibuat untuk memenuhi tugas Ujian Tengah Semester
mata kuliah Data Acquisition and Management.

Proyek berfokus pada proses pengumpulan, pengolahan, pemeriksaan,
dan penggabungan data pada sektor pariwisata, khususnya objek
wisata belanja di Kota Bandung.

Pengumpulan data dilakukan melalui tiga metode:
1. Mengunduh dataset dari portal data terbuka.
2. Mengambil data melalui API Open-Meteo.
3. Melakukan web scraping pada situs TIC Bandung dengan
   memperhatikan ketentuan robots.txt.

### 3. Sumber Data

**A. Dataset utama**

- Nama: Objek Wisata Belanja di Kota Bandung
- Sumber: data.go.id
- URL: https://data.go.id/dataset/dataset/objek-wisata-belanja-di-kota-bandung

**B. API**

- Nama: Open-Meteo API
- URL: https://api.open-meteo.com/v1/forecast
- Data: Informasi cuaca berdasarkan waktu dan lokasi Bandung.

**C. Web Scraping**

- Nama situs: TIC Bandung
- URL: https://www.ticbandung.com/kategori
- Data: Informasi kategori atau daftar terkait pariwisata.

### 4. Struktur Folder

```text
UTS_DAM_Wisata_Bandung/
│
├── data/
│   ├── raw/
│   │   ├── objek_wisata_belanja_di_kota_bandung_2.csv
│   │   ├── openmeteo_raw.json
│   │   ├── tic_bandung_raw.html
│   │   └── tic_bandung_robots.txt
│   │
│   └── processed/
│       ├── data_gabungan.csv
│       ├── hasil_merge.csv
│       ├── openmeteo_weather.csv
│       └── tic_bandung_listing.csv
│
├── docs/
│   ├── evidence/
│   │   └── tic_robots_check.json
│   ├── data_dictionary.csv
│   ├── data_ethics_checklist.csv
│   ├── provenance.csv
│   └── robots_rules_reported_by_user.txt
│
├── notebooks/
│   └── UTS_DAM_Bandung.ipynb
│
├── outputs/
│   └── metadata_merge.json
│
└── README.md
