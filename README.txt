# 📑 Tambah Usaha Matchapro

Script otomasi berbasis Python untuk melakukan upload data usaha secara massal ke platform **Matchapro BPS**. Alat ini dilengkapi dengan fitur login SSO, manajemen OTP, bypass deteksi desktop (Mobile Emulation), dan penanganan rate limit otomatis.

---

## 🛠 Persyaratan Sistem (Prasyarat)
Sebelum menjalankan script atau membangun file `.exe`, pastikan perangkat memiliki:
* **Python 3.9+**
* **Google Chrome** (Atau browser berbasis Chromium lainnya).
* **File Pendukung (Wajib dalam satu folder):**
    * `loginX.py` (Modul login SSO).
    * `desa.xlsx` (Database master kode wilayah).
    * File input data usaha (format `.xlsx`).

---

## 🚀 Instalasi & Persiapan
1. **Clone atau Copy Script** ke dalam satu folder.
2. **Instal Dependensi:**
   ```bash
   pip install pandas requests playwright pyotp psutil openpyxl

---

## 📖 Cara Penggunaan
Pastikan file desa.xlsx dan file data Anda berada di folder yang sama dengan script.
1. Jalankan script: python tambahBaru.py
2. Masukkan Username dan Password SSO BPS Anda.
3. Masukkan kode OTP jika diminta.
4. Ketikkan nama file excel target (tanpa ekstensi .xlsx).
5. Masukkan indeks baris mulai (ketik 0 jika ingin dari awal).
6. Pantau progress di terminal.