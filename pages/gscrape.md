# GScrape
# Dokumentasi Penggunaan gscrape.py

## Pendahuluan
Silahkan unduh aplikasi pada link berikut ==>>[unduh aplikasi](https://drive.bps.go.id/s/LP7KyjwzPgeGYqn)

`gscrape.py` adalah sebuah script Python yang digunakan untuk melakukan web scraping data dari Google Maps. Script ini dapat dijalankan melalui terminal dengan berbagai parameter untuk menyesuaikan jumlah halaman dan batas data yang ingin dikumpulkan.

## Instalasi
Sebelum menjalankan `gscrape.py`, pastikan sistem Anda telah terinstal Python dan dependensi yang dibutuhkan. Jika belum, instal dependensi dengan perintah berikut:

```bash
pip install -r requirements.txt
```

## Cara Menjalankan Script
Script `gscrape.py` dapat dijalankan dengan menggunakan perintah berikut di terminal:

```bash
python gscrape.py --page <jumlah_halaman> --limit <batas_data> --sumber <sumber_data> --file <sumber_data>
```

### Parameter
- `--page`: Menentukan jumlah halaman yang akan di-scrape. Contoh: `--page 1` berarti hanya mengambil data dari halaman pertama.
- `--limit`: Menentukan jumlah maksimal data yang akan diambil. Contoh: `--limit 1000` berarti akan mengambil maksimal 1000 data.
- `--sumber`: Menentukan sumber data yang akan diambil. Contoh: `--sumber kadin` akan mengambil data berdasarkan sumber "kadin".
- `--file`: Menentukan apakah menggunakan file excel pencarian atau dari API server. Contoh: `--file y` akan mengambil data dari file pencarian.xlsx.

### Contoh Penggunaan
Misalkan Anda ingin mengambil 1000 data dari halaman pertama dengan sumber "kadin", jalankan perintah berikut:

```bash
python gscrape.py --page 1 --limit 1000 --sumber kadin
```

## Output
Script akan menghasilkan output dalam format XLSX atau CSV, tergantung pada pengaturan dalam script. Output akan tersimpan dalam folder yang sama dengan script ini.

## Troubleshooting
1. **ModuleNotFoundError**: Pastikan Anda telah menginstal semua dependensi dengan `pip install -r requirements.txt`.
2. **Data tidak ditemukan**: Pastikan parameter yang diberikan sesuai dan koneksi internet stabil.
3. **Akses ditolak atau CAPTCHA muncul**: Gunakan rotating proxies atau sesuaikan frekuensi scraping untuk menghindari deteksi bot.

## Catatan
- Gunakan script ini secara bertanggung jawab dan patuhi kebijakan layanan Google Maps.

## Pengembang
Script ini dikembangkan untuk kebutuhan scraping data infrastruktur dari Google Maps. Untuk pengembangan lebih lanjut atau perbaikan bug, silakan chat melalui kolom issue.

---
**Versi Script:** 1.0  
**Tanggal Rilis:** Februari 2025

