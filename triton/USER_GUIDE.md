### Daftar Isi
- [Home](#home)
    - [Login](#login)
    - [Lupa Password](#lupa-password)
- [Dasbor](#dasbor)
    - [Ringkasan](#ringkasan)
    - [Performa](#performa)
    - [Grafik Harian](#grafik-harian)
- [Surat Masuk](#surat-masuk)
    - [Filter Surat Masuk](#filter-surat-masuk)
    - [Surat Masuk Baru](#surat-masuk-baru)
    - [Aksi Surat Masuk](#aksi-surat-masuk)
    - [Detail Surat Masuk](#detail-surat-masuk)

## Home

Jika Anda tertarik dengan produk kami yang lain bisa kunjungi GitHub kami atau kontak langsung via email di [404nf.oa@gmail.com](mailto:404nf.oa@gmail.com).

![Home](./ss/Screenshot%202025-05-18%20at%2005.53.35.png)

### Login

Diisi dengan email dan password Anda, Anda bisa menggunakan [akun bawaan](./installation.md#login).

![Login](./ss/Screenshot%202025-05-18%20at%2005.53.57.png)

Jika _Remember me_ ditandai maka browser akan mengingat sesi login Anda.

### Lupa Password

Jika Anda lupa password silakan isi email Anda nanti akan ada email masuk yang berisikan link untuk reset password.

![Lupa Password](./ss/Screenshot%202025-05-18%20at%2005.54.13.png)


## Dasbor

Ini adalah panel utama dan merupakan kesimpulan dari apa yang terjadi di aplikasi Anda.

![Dasbor](./ss/Screenshot%202025-05-18%20at%2005.54.40.png)

Secara garis besar ada tiga bagian pada halaman dasbor ini:
- **Ringkasan**: ringkasan dari isi aplikasi, sepanjang waktu
- **Performa**: difilter berdasarkan bulan
- **Grafik Harian**: difiliter berdasarkan bulan

Di bawah ringkasan terdapat filter bulan yang digunakan untuk memilih bulan yang ditampilkan pada **Performa** dan **Grafik Harian**.

![Filter Bulan Dasbor](./ss/Screenshot%202025-05-18%20at%2005.54.47.png)

### Ringkasan

Di bagian ini ada 4 ringkasan:
- **Surat Masuk**
- **Surat Keluar**
- **Belum Diproses**: Surat masuk yang belum mempunyai disposisi
- **Perlu Diproses**: Disposisi yang harus dibuatkan surat balasannya

### Performa

Di bagian ini ada 3:
- **Rata-rata waktu proses**
- **Ketepatan waktu disposisi**
- **Konversi disposisi ke surat keluar**

### Grafik Harian

atau **Statistik** menggambarkan transaksi harian antara Surat Masuk, Surat Keluar, dan Disposisi pada sistem.


## Surat Masuk

Panel surat masuk berisikan data surat masuk yang diurutkan berdasarkan surat terbaru yang disimpan ke dalam aplikasi.

![Surat Masuk](./ss/Screenshot%202025-05-18%20at%2006.47.29.png)

Secara berurutan data yang ditampilkan pada setiap baris adalah berikut:
- **Nomor Agenda**: penomoran unik pada setiap surat yang tersusun atas kode (`M`/`K`), nomor urut surat, bulan dalam romawi, dan tahun.
- **Pengirim**
- **Perihal dan Isi**
- **Waktu Disimpan**: waktu menunjukkan kapan surat diterima atau disimpan ke dalam aplikasi

Surat yang **belum dibaca** ditunjukkan dengan **cetak tebal** sedangkan surat yang **sudah dibaca** ditunjukkan dengan **warna baris yang agak gelap**. 

Di sebelah kiri **Nomor Agenda** terkadang akan muncul ikon indikator.
- Ikon komentar mengindikasikan bahwa surat sudah memiliki disposisi.
    ![Disposisi](./ss/Screenshot%202025-05-18%20at%2006.47.47.png)
- Ikon pesawat kertas mengindikasikan bahwa surat sudah dibalas
    ![Dibalas](./ss/Screenshot%202025-05-18%20at%2006.48.19.png)

### Filter Surat Masuk

Anda bisa menyaring surat masuk yang ingin ditampilkan.

![Filter](./ss/Screenshot%202025-05-18%20at%2006.50.52.png)

Selain itu juga hasil penyaringan tersebut bisa diekspor ke file `csv` yang dapat dibuka baik di Excel maupun Google Spreadsheet. File tersebut akan dikirimkan melalui email.

### Surat Masuk Baru

![Surat Masuk Baru](./ss/Screenshot%202025-05-18%20at%2006.52.28.png)

Ketika ingin membuat surat masuk baru Anda harus mengunggah file (pdf atau gambar) dari surat tersebut sebagai arsip.

![Surat Masuk Baru](./ss/Screenshot%202025-05-18%20at%2006.53.46.png)

Setelah file diunggah Anda akan diperlihatkan file surat beserta form inputan dari surat yang bisa Anda isi secara manual. 

![AI](./ss/Screenshot%202025-05-18%20at%2006.55.00.png)

Opsi lain Anda bisa menggunakan AI✨ untuk **mengisikan datanya** untuk Anda sekaligus memberikan **rangkuman surat** beserta rekomendasi untuk **kategori surat**.

![AI Process](./ss/Screenshot%202025-05-18%20at%2006.54.03.png)

![AI Result](./ss/Screenshot%202025-05-18%20at%2006.54.29.png)

Di form tersebut tidak ada **Nomor Agenda**, karena akan dibuatkan secara otomatis oleh sistem dan bersifat internal.

### Aksi Surat Masuk

Jika Anda mengarahkan pointer atau cursor ke baris surat maka **Waktu Disimpan** akan menampilkan aksi yang bisa dilakukan terhadap surat.

![Download](./ss/Screenshot%202025-05-18%20at%2006.48.50.png)
Aksi **Unduh** digunakan untuk mengunduh berkas surat masuk.

![Edit](./ss/Screenshot%202025-05-18%20at%2006.49.27.png)
Aksi **Edit** digunakan untuk mengedit berkas.

![Mark As Unread](./ss/Screenshot%202025-05-18%20at%2006.49.48.png)
Aksi **Tandai Belum Dibaca** hanya dapat dilakukan pada surat yang sudah dibaca.

![Delete](./ss/Screenshot%202025-05-18%20at%2006.50.18.png)
Aksi **Hapus** digunakan untuk menghapus surat.

### Detail Surat Masuk

![Detail Surat Masuk](./ss/Screenshot%202025-05-18%20at%2011.43.28.png)