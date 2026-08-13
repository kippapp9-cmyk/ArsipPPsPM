# Monitoring Pemindaian SPM — Google Sheets

File `index_google_sheets.html` sudah memiliki integrasi Google Sheets.

## 1. Buat database Google Sheet
Buat Google Sheet baru, misalnya `Database Monitoring SPM`.

## 2. Pasang Apps Script
Di Google Sheet pilih **Extensions → Apps Script**.
Ganti isi `Code.gs` dengan file `Code.gs` yang disertakan.

## 3. Deploy Web App
Pilih **Deploy → New deployment → Web app**:
- Execute as: **Me**
- Who has access: **Anyone** (atau pengaturan akses yang sesuai kebijakan organisasi)

Klik Deploy dan salin URL yang berakhiran `/exec`.

## 4. Hubungkan HTML
Buka `index_google_sheets.html`, klik **☁ Google Sheets**, lalu tempel URL Web App.
URL akan disimpan di browser.

## 5. Sinkronisasi
- **Muat dari Sheets**: mengambil data dari Google Sheet.
- **Simpan ke Sheets**: mengganti isi database Google Sheet dengan data aplikasi.
- Setelah URL tersimpan, penambahan/edit/penghapusan data akan mencoba melakukan sinkronisasi otomatis ke Google Sheets.

## Catatan keamanan
Jangan memasukkan data rahasia ke Web App yang dibuka untuk publik. Jika aplikasi digunakan hanya di lingkungan BPS/organisasi, sebaiknya gunakan pembatasan akses Google Workspace yang sesuai.
