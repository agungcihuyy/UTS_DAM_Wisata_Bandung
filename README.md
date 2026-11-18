# UTS DAM — Pariwisata / Objek Wisata Belanja Kota Bandung

Paket ini disusun mengikuti PDF UTS DAM Kelas E (Soal 1–5).

## Isi folder
- `data/raw/`: sumber mentah yang tidak diubah. Saat paket dibuat sudah berisi CSV Bandung asli.
- `data/processed/`: hasil normalisasi, CSV API, hasil scraping, dan hasil merge setelah notebook dijalankan.
- `notebooks/UTS_DAM_Bandung.ipynb`: satu notebook utama untuk semua soal.
- `docs/`: data dictionary, checklist etika, provenance, catatan robots, dan perbandingan dengan notebook contoh.
- `outputs/`: tempat keluaran tambahan.

## Dataset yang sudah tersedia
- Baris x kolom: 326 x 10
- Ukuran: 43370 byte
- MD5: `86fd1df3bf4f81c89d288857c7e41337`
- File raw disalin apa adanya.
- **PENTING:** URL portal asal dan lisensi belum diverifikasi. PDF mensyaratkan dataset terbuka dari BPS, Satu Data Bali, data.go.id, atau Kaggle dan minimal 100 baris. Pastikan sumber file ini memenuhi ketentuan tersebut.

## Cara menjalankan
1. Upload/ekstrak folder `UTS_DAM_Bandung` ke `MyDrive` Google Drive.
2. Buka `notebooks/UTS_DAM_Bandung.ipynb` dengan Google Colab.
3. Jalankan semua sel dari atas ke bawah.
4. Ganti `EMAIL_KAMPUS` dengan email kampus.
5. Periksa URL dan lisensi dataset utama; jangan biarkan placeholder pada provenance.
6. Periksa bahwa `Shopping & Fashion` benar-benar terambil dari halaman TIC dan merge sukses. Jika tidak, jangan mengarang relasi.
7. Pastikan `data/raw` berisi CSV, JSON API, HTML TIC, dan robots TIC setelah notebook selesai.
8. Pastikan hasil `data/processed/data_gabungan.csv`, checklist, provenance, dan bukti robots tersedia.

**Paket ini belum merupakan tugas final yang seluruhnya selesai:** data API/TIC baru diperoleh saat notebook dijalankan. Tidak ada data mentah API/scraping yang dibuat-buat.
