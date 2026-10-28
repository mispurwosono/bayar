# 🕌 Aplikasi Pembayaran Siswa MI Nurul Islam Purwosono

Sistem informasi & administrasi keuangan siswa terpadu untuk **MI Nurul Islam Purwosono** (Kelas 1 s.d. 6). Dirancang dengan tampilan modern, dominan hijau khas madrasah, responsif otomatis menyesuaikan layar laptop maupun smartphone, serta dilengkapi sistem autentikasi **Login Admin vs Siswa** dan integrasi **Google Spreadsheet**.

---

## 🌟 Fitur Utama Aplikasi

### 1. Menu Tampilan Awal (Portal Login 2 Jalur)
* **Login Siswa / Wali Murid**:
  - Masuk cukup dengan memasukkan **NIS (Nomor Induk Siswa)**.
  - Terdapat pilihan cepat (*quick select*) untuk mempermudah wali murid menemukan nama putranya.
  - **Dashboard Khusus Siswa**: Wali murid dapat mengecek saldo tabungan, riwayat pembayaran infaq & LKS yang telah lunas, dan langsung mencetak bukti kuitansi resmi tanpa bisa mengubah data.
* **Login Admin / Bendahara MI**:
  - Masuk menggunakan **PIN Keamanan Admin** (PIN bawaan default: **`123456`**).
  - PIN dapat diubah kapan saja melalui menu pengaturan.
  - Membuka akses penuh ke kasir, buku tabungan (setor/tarik), rekapitulasi, data siswa, dan integrasi spreadsheet.

---

### 2. Fitur Kasir & Administrasi (Admin)
* **Pembayaran Tagihan**:
  - Infaq Bulanan (pilihan bulan Juli - Juni).
  - LKS Tematik Semester (nominal otomatis mendeteksi kelas 1 s.d. 6).
  - Infaq Pembangunan Gedung, Ujian Semester, dan biaya kustom.
  - Kalkulator kembalian uang kasir otomatis.
* **Buku Tabungan Siswa**:
  - Setor (+) dan Tarik (-) dengan validasi saldo.
  - Riwayat mutasi tabungan *real-time*.
* **Laporan & Ekspor**:
  - Rekapitulasi per kelas dan filter kata kunci.
  - Ekspor seluruh laporan transaksi ke format **Excel / CSV**.
* **Manajemen Siswa**:
  - Direktori siswa kelas 1-6 dan formulir penambahan siswa baru.

---

### 3. Kuitansi Resmi & Notifikasi WhatsApp
* Kuitansi cetak resmi lengkap dengan Kop Madrasah, Nomor Transaksi, tanggal, terbilang bahasa Indonesia (*"Dua Puluh Lima Ribu Rupiah"*), stempel lunas, dan tanda tangan bendahara.
* Tombol **Kirim ke WhatsApp**: otomatis membuka chat WA wali murid dengan format bukti lunas yang rapi.

---

### 4. Visual & Responsif
* **Mode Hijau (Islamic Deep Emerald)**: Nuansa hijau madrasah mewah dan nyaman di mata.
* **Mode Cerah (Light Mode)**: Nuansa bersih cerah dengan aksen hijau emerald.
* **Responsif Otomatis**: Tampilan otomatis menyesuaikan layar monitor komputer, laptop, tablet, hingga smartphone Android / iOS.

---

## 🚀 Cara 1: Buka & Coba Langsung di Komputer (Offline/Lokal)

1. Buka folder `d:\Projek` di file explorer komputer Anda.
2. Klik dua kali file **`index.html`**.
3. Di layar awal:
   - Pilih **Siswa** dan masukkan NIS contoh (misal: `20240101` untuk Ahmad Zaki Fauzi Kelas 1).
   - Atau pilih **Admin** dan masukkan PIN: `123456`.

---

## 🌐 Cara 2: Upload ke Vercel agar Bisa Diakses Publik Secara Gratis

1. Masuk ke [https://vercel.com](https://vercel.com) dengan akun Google Anda.
2. Buat repositori baru di [GitHub](https://github.com) (misal: `pembayaran-mi-nurul-islam`) dan unggah seluruh file di folder `d:\Projek`.
3. Di dashboard Vercel, klik **"Add New..."** > **"Project"** > pilih repositori Anda > klik **"Deploy"**.
4. Dalam 30 detik web publik Anda sudah aktif secara gratis!

---

## 📊 Cara Menghubungkan ke Google Spreadsheet Sekolah

1. Buka [Google Sheets baru](https://sheets.new) di akun Google madrasah. Beri nama: `DB_Pembayaran_MI_Nurul_Islam`.
2. Buka menu **Ekstensi > Apps Script**.
3. Salin kode dari file [google-apps-script/Code.gs](file:///d:/Projek/google-apps-script/Code.gs) dan tempel ke editor.
4. Pilih fungsi **`initSheets`** lalu klik tombol **Jalankan (Run)** untuk membuat seluruh tabel otomatis.
5. Klik **Terapkan (Deploy) > Penerapan Baru > Aplikasi Web**:
   - Siapa yang memiliki akses: pilih **"Siapa saja (Anyone)"**.
6. Salin tautan **URL Web App**, masuk ke aplikasi web Anda di menu **Pengaturan & Spreadsheet**, lalu klik **Simpan & Uji Koneksi**.

---

*Dikembangkan untuk MI Nurul Islam Purwosono.*
