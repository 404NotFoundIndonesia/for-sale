<div align="center">
    <a href="https://404notfound.fun" target="_blank">
        <img src="../404NFID-green.png" 
            width="100" 
            alt="404NFID Logo">
    </a>
</div>

# Triton - Aplikasi Manajemen Surat

### Daftar Isi

- [Deskripsi Produk](#deskripsi-produk)
- [Tujuan](#tujuan)
- [Fitur Utama](#fitur-utama)
  - [Akun](#akun-pengguna)
  - [Dashboard](#dashboard)
  - [Surat Masuk](#surat-masuk)
  - [Surat Keluar](#surat-keluar)
  - [Kategori Surat](#kategori-surat)
  - [Manajemen Pengguna](#manajemen-pengguna)
  - [Jabatan](#jabatan)
- [Teknologi](#teknologi)
- [Rancangan](#rancangan)
- [Instalasi](#instalasi)
- [Screenshot](#screenshot)
- [License](#license)

## Deskripsi Produk
Triton adalah aplikasi berbasis web untuk mengelola surat masuk dan keluar, dilengkapi dengan fitur AI untuk ekstraksi data otomatis, klasifikasi isi, ringkasan, dan saran disposisi. Aplikasi ini dibangun menggunakan Laravel di sisi backend dan Vue.js di sisi frontend.

## Tujuan
- Meningkatkan efisiensi dan akurasi dalam pengelolaan surat.
- Mengurangi beban input manual dengan bantuan AI.
- Menyediakan sistem manajemen disposisi yang terorganisir.

## Fitur Utama

### Akun Pengguna

- Login & Lupa Kata Sandi
- Update profil dan ubah/reset kata sandi
- Ganti bahasa: `id`, `en`, `ja`, `ko`, `ar`, `zh-CN`
- Lihat dan hapus sesi login aktif
- Hapus akun secara mandiri

### Dashboard

- Ringkasan:
  - Total surat masuk & keluar
  - Jumlah surat masuk yang belum diproses
  - Jumlah surat masuk yang harus diproses
- Statistik performa:
  - Rata-rata waktu proses surat bulanan
  - Ketepatan waktu penyelesaian disposisi bulanan
  - Tingkat konversi disposisi ke surat keluar per bulan
- Grafik harian (bar chart):
  - Surat masuk, surat keluar, dan disposisi

### Surat Masuk

- CRUD surat masuk
- Upload file (pdf atau gambar) → Ekstrak data otomatis (opsional)
- Ringkasan isi surat dengan AI
- Rekomendasi kategori otomatis menggunakan AI
- Tandai surat sebagai belum dibaca
- Filter surat:
  - Sudah dibaca / Belum dibaca
  - Surat belum diproses
  - Surat harus diproses
- Disposisi:
  - CRUD disposisi
  - Rekomendasi isi disposisi dari AI
  - Kirim email otomatis ke penerima disposisi
  - Email pemberitahuan saat disposisi selesai
- Surat balasan:
  - Buat surat keluar sebagai balasan dari surat masuk
- Ekspor data ke CSV (dikirim via email)

### Surat Keluar

- CRUD surat keluar
- Upload file (pdf atau gambar) → Ekstrak data otomatis (opsional)
- Ringkasan isi surat dengan AI
- Rekomendasi kategori otomatis menggunakan AI
- Filter surat keluar
- Ekspor data ke CSV (dikirim via email)

### Kategori Surat

- CRUD kategori surat untuk mengorganisasi surat masuk & keluar

### Manajemen Pengguna

- CRUD pengguna
- Kirim email otomatis berisi password saat pengguna dibuat

### Jabatan

- CRUD jabatan
- Digunakan untuk pembatasan hak akses ke fitur-fitur aplikasi
- Hak akses yang tersedia:
    - **Pengguna**: `ViewUser`, `AddUser`, `EditUser`, `DeleteUser`
    - **Jabatan**:  `ViewRole`, `AddRole`, `EditRole`, `DeleteRole`
    - **Surat Masuk**: `ViewIncomingLetter`, `AddIncomingLetter`, `EditIncomingLetter`, `DeleteIncomingLetter`
    - **Surat Keluar**: `ViewOutgoingLetter`, `AddOutgoingLetter`, `EditOutgoingLetter`, `DeleteOutgoingLetter`
    - **Kategori Surat**: `ViewLetterCategory`, `AddLetterCategory`, `EditLetterCategory`, `DeleteLetterCategory`
    - **Disposisi**: `ViewDisposition`, `AddDisposition`, `EditDisposition`, `DeleteDisposition`

## Teknologi

- **Laravel 12** – Backend API
- **Vue 3 + Vite** – Reactive frontend
- **Tailwind CSS** – Utility-first CSS framework
- **MySQL** – Relational database
- **Gemini** - AI Agent

## Rancangan

Untuk rancangan aplikasi silakan merujuk ke halaman [blueprint](./blueprint.md).

## Instalasi

Untuk instalasi aplikasi silakan merujuk ke halaman [installation](./installation.md).

## User Guide

Anda bisa melihat dokumentasi atau cara penggunaan Triton di halaman [user guide](./USER_GUIDE.md).

## Screenshot

![Home](ss/Screenshot%202025-05-18%20at%2005.53.35.png)
![Dashboard](ss/Screenshot%202025-05-18%20at%2005.54.40.png)
![Inbox](ss/Screenshot%202025-05-18%20at%2006.47.29.png)

## License

This project is proprietary software.  
© 2025 [404NotFoundIndonesia](https://github.com/404NotFoundIndonesia) – All rights reserved.  
Use of this software is governed by the [Triton Software License Agreement](LICENSE).