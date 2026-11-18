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
UTS_DAM_Bandung/
│
├── data/
│   ├── raw/
│   │   ├── dataset_bandung.csv
│   │   ├── openmeteo_raw.json
│   │   └── ticbandung_raw.html
│   │
│   └── processed/
│       ├── openmeteo_weather.csv
│       ├── ticbandung_listing.csv
│       └── hasil_merge.csv
│
├── docs/
│   ├── provenance.csv
│   ├── data_ethics_checklist.csv
│   └── evidence/
│      └──tic_robots_check.json
│
├── notebooks/
│   └── UTS_DAM_Bandung.ipynb
│
├── README.md
└── outputs/
    └── metadata_merge.json
