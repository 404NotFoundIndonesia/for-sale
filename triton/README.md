<div align="center">
    <a href="https://404notfound.fun" target="_blank">
        <img src="../404NFID-green.png" 
            width="100" 
            alt="404NFID Logo">
    </a>
</div>

# Triton - Aplikasi Manajemen Surat

## Deskripsi Produk
Triton adalah aplikasi berbasis web untuk mengelola surat masuk dan keluar, dilengkapi dengan fitur AI untuk ekstraksi data otomatis, klasifikasi isi, ringkasan, dan saran disposisi. Aplikasi ini dibangun menggunakan Laravel di sisi backend dan Vue.js di sisi frontend.

## Tujuan
- Meningkatkan efisiensi dan akurasi dalam pengelolaan surat.
- Mengurangi beban input manual dengan bantuan AI.
- Menyediakan sistem manajemen disposisi yang terorganisir.

## Fitur Utama

### 📥 Surat Masuk
- Upload dokumen (PDF, JPG, PNG).
- **Ekstraksi Otomatis oleh AI**: Isi metadata surat (nomor, tanggal, pengirim, perihal).
- **Klasifikasi Surat Otomatis**: AI menyarankan kategori surat.
- **Ringkasan Surat Otomatis**: Ditampilkan untuk pratinjau cepat.
- Disposisi saran dari AI.
- Riwayat dan status surat terpantau.

### 📤 Surat Keluar
- Pembuatan draft dan unggah dokumen.
- Penomoran otomatis.
- **AI Ringkasan Surat** untuk efisiensi review.

### 🔄 Disposisi
- Disposisi ke pengguna lain.
- AI memberikan **saran disposisi** berdasarkan isi surat.
- Riwayat dan pelacakan proses.

### 📁 Kategori Surat
- AI menyarankan kategori saat input surat.

### 👤 Manajemen Pengguna
- CRUD pengguna dan pengaturan role.
- Role bersifat **dinamis** (bisa ditambah/ubah).
- Permission bersifat **statis**, digunakan di `Gate` Laravel.

### 🔐 Role & Permission
- Role dapat dikonfigurasi admin.
- Permission statis dan digunakan untuk kontrol akses (Gate di Laravel, directive di Vue).

### 🔍 Pencarian & Filter
- Pencarian berdasarkan metadata dan isi surat.
- Filter berdasarkan tanggal, perihal, dan status.

### 📊 Laporan
- Export CSV untuk surat masuk & keluar, dikirim ke email.
- Disertai filter berdasarkan waktu, perihal, dan status.

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

## 📸 Screenshot

![Home](ss/Screenshot%202025-05-18%20at%2005.53.35.png)
![Dashboard](ss/Screenshot%202025-05-18%20at%2005.54.40.png)
![Inbox](ss/Screenshot%202025-05-18%20at%2006.47.29.png)

## 📄 License

This project is proprietary software.  
© 2025 [404NotFoundIndonesia](https://github.com/404NotFoundIndonesia) – All rights reserved.  
Use of this software is governed by the [Triton Software License Agreement](LICENSE).