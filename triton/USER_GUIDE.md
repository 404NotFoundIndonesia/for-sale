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
    - [Disposisi](#disposisi)
- [Surat Keluar](#surat-keluar)
    - [Filter Surat Keluar](#filter-surat-keluar)
    - [Surat Keluar Baru](#surat-keluar-baru)
    - [Aksi Surat Keluar](#aksi-surat-keluar)
    - [Detail Surat Keluar](#detail-surat-keluar)
- [Kategori Surat](#kategori-surat)
- [Manajemen Pengguna](#pengguna)
- [Jabatan](#jabatan)
- [Pengaturan](#pengaturan)
    - [Profil](#profil)
    - [Kata Sandi](#kata-sandi)
    - [Sesi](#sesi)
    - [Tampilan](#tampilan)

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
- **Nomor Agenda**: penomoran unik pada setiap surat yang tersusun atas kode (`M`), nomor urut surat, bulan dalam romawi, dan tahun.
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

![Filter](./ss/Screenshot%202025-05-18%20at%2016.22.26.png)

Selain itu juga hasil penyaringan tersebut bisa diekspor ke file `csv` yang dapat dibuka baik di Excel maupun Google Spreadsheet. File tersebut akan dikirimkan melalui email.

### Surat Masuk Baru

Ketika ingin membuat surat masuk baru Anda harus mengunggah file (pdf atau gambar) dari surat tersebut sebagai arsip.

![Surat Masuk Baru](./ss/Screenshot%202025-05-18%20at%2006.52.28.png)

Setelah file diunggah Anda akan diperlihatkan file surat beserta form inputan dari surat yang bisa Anda isi secara manual. 

![Surat Masuk Baru](./ss/Screenshot%202025-05-18%20at%2006.53.46.png)

Opsi lain Anda bisa menggunakan AI✨ untuk **mengisikan datanya**  sekaligus memberikan **rangkuman surat** beserta rekomendasi untuk **kategori surat**.

![AI](./ss/Screenshot%202025-05-18%20at%2006.55.00.png)

![AI Process](./ss/Screenshot%202025-05-18%20at%2006.54.03.png)

![AI Result](./ss/Screenshot%202025-05-18%20at%2006.54.29.png)

Di form tersebut tidak ada **Nomor Agenda**, karena akan dibuatkan secara otomatis oleh sistem dan bersifat internal.

### Aksi Surat Masuk

Jika Anda mengarahkan pointer atau cursor ke baris surat maka **Waktu Disimpan** akan menampilkan aksi yang bisa dilakukan terhadap surat.

Aksi **Unduh** digunakan untuk mengunduh berkas surat masuk.

![Download](./ss/Screenshot%202025-05-18%20at%2006.48.50.png)

Aksi **Edit** digunakan untuk mengedit berkas.

![Edit](./ss/Screenshot%202025-05-18%20at%2006.49.27.png)

Aksi **Tandai Belum Dibaca** hanya dapat dilakukan pada surat yang sudah dibaca.

![Mark As Unread](./ss/Screenshot%202025-05-18%20at%2006.49.48.png)

Aksi **Hapus** digunakan untuk menghapus surat.

![Delete](./ss/Screenshot%202025-05-18%20at%2006.50.18.png)

Selain empat aksi di atas, Anda juga bisa melakukan _bulk action_ dengan menandai surat.

![Bulk](./ss/Screenshot%202025-05-18%20at%2011.50.10.png)

_Bulk action_ hanya akan muncul ketika ada surat yang dipilih.

### Detail Surat Masuk

Ketika Anda membuka surat masuk, akan seperti ini tampilannya.

![Detail Surat Masuk](./ss/Screenshot%202025-05-18%20at%2011.43.28.png)

Jika surat masuk sudah dibalas, maka di bagian bawah akan ada nomor agenda surat keluar yang berkaitan.

![Surat Masuk Balasan](./ss/Screenshot%202025-05-18%20at%2014.13.25.png)

### Disposisi

Untuk membuat disposisi surat, Anda bisa klik tombol disposisi yang ada di kanan atas layar.

![Disposisi Baru](./ss/Screenshot%202025-05-18%20at%2013.34.23.png)

Anda dapat menugaskan pengguna lain untuk mengerjakan disposisi. Jika disposisi memerlukan surat balasan, maka Anda dapat menetapkan tenggat waktunya.

![Form Disposisi](./ss/Screenshot%202025-05-18%20at%2013.36.44.png)

Anda juga dapat meminta rekomendasi oleh AI✨ perlu diapakan surat ini.

![Rekomendasi AI](./ss/Screenshot%202025-05-18%20at%2013.40.13.png)

Pengguna yang ditugaskan akan menerima email penugasan disposisi.

![Form Disposisi](./ss/Screenshot%202025-05-18%20at%2013.45.13.png)

Setelah disposisi berhasil dibuat, semua disposisi akan ditampilkan di bagian bawah surat masuk.

![Konten Disposisi](./ss/Screenshot%202025-05-18%20at%2013.47.30.png)

Satu surat bisa memiliki banyak disposisi dan satu disposisi juga bisa memiliki disposisi terusan. 

Di bagian atas disposisi ada pengguna yang memberi disposisi dan yang ditugaskan untuk mengurus disposisi. Nama yang diberi warna hijau terang adalah akun pengguna yang sedang login. Jika tidak ada yang ditugaskan atas disposisi, maka hanya nama pengguna yang membuat disposisi yang akan tampil.

Di bagian pojok kanan bawah ada indikasi penyelesaian disposisi. Disposisi yang telah selesai akan berwarna hijau dan jika ada surat keluar berdasarkan disposisi tersebut maka di sebelahnya akan tampil pula nomor agenda surat keluarnya.

![Disposisi Selesai](./ss/Screenshot%202025-05-18%20at%2013.54.50.png)

Pengguna yang ditugaskan mengurus disposisi bisa membuat surat balasan berdasarkan disposisi bersangkutan.

![Aksi Disposisi](./ss/Screenshot%202025-05-18%20at%2014.10.08.png)

Alur pembuatan surat balasan sama dengan [pembuatan surat keluar baru](#surat-keluar-baru).

## Surat Keluar
Panel surat keluar berisikan data surat keluar yang diurutkan berdasarkan surat terbaru yang disimpan ke dalam aplikasi.

![Surat Keluar](./ss/Screenshot%202025-05-18%20at%2013.59.39.png)

Secara berurutan data yang ditampilkan pada setiap baris adalah berikut:
- **Nomor Agenda**: penomoran unik pada setiap surat yang tersusun atas kode (`K`), nomor urut surat, bulan dalam romawi, dan tahun.
- **Penerima**
- **Perihal dan Isi**
- **Waktu Disimpan**: waktu menunjukkan kapan surat diunggah atau disimpan ke dalam aplikasi

### Filter Surat Keluar

Anda bisa menyaring surat keluar yang ingin ditampilkan.

![Filter](./ss/Screenshot%202025-05-18%20at%2016.31.59.png)

Selain itu juga hasil penyaringan tersebut bisa diekspor ke file `csv` yang dapat dibuka baik di Excel maupun Google Spreadsheet. File tersebut akan dikirimkan melalui email.

### Surat Keluar Baru

Ketika ingin membuat surat keluar baru Anda harus mengunggah file (pdf atau gambar) dari surat tersebut sebagai arsip.

![Surat Keluar Baru](./ss/Screenshot%202025-05-18%20at%2014.03.23.png)

Setelah file diunggah Anda akan diperlihatkan file surat beserta form inputan dari surat yang bisa Anda isi secara manual. 

![Surat Keluar Baru](./ss/Screenshot%202025-05-18%20at%2014.04.23.png)

Opsi lain Anda bisa menggunakan AI✨ untuk **mengisikan datanya**  sekaligus memberikan **rangkuman surat** beserta rekomendasi untuk **kategori surat**.

![AI](./ss/Screenshot%202025-05-18%20at%2006.55.00.png)

![AI Result](./ss/Screenshot%202025-05-18%20at%2014.05.09.png)

Di form tersebut tidak ada **Nomor Agenda**, karena akan dibuatkan secara otomatis oleh sistem dan bersifat internal.

### Aksi Surat Keluar

Jika Anda mengarahkan pointer atau cursor ke baris surat maka **Waktu Disimpan** akan menampilkan aksi yang bisa dilakukan terhadap surat.

Aksi **Unduh** digunakan untuk mengunduh berkas surat keluar.

![Download](./ss/Screenshot%202025-05-18%20at%2014.06.00.png)

Aksi **Edit** digunakan untuk mengedit berkas.

![Edit](./ss/Screenshot%202025-05-18%20at%2014.06.23.png)

Aksi **Hapus** digunakan untuk menghapus surat.

![Delete](./ss/Screenshot%202025-05-18%20at%2014.06.42.png)

Selain empat aksi di atas, Anda juga bisa melakukan _bulk action_ dengan menandai surat.

![Bulk](./ss/Screenshot%202025-05-18%20at%2014.07.01.png)

_Bulk action_ hanya akan muncul ketika ada surat yang dipilih.

### Detail Surat Keluar

Ketika Anda membuka surat keluar, akan seperti ini tampilannya.

![Detail Surat Keluar](./ss/Screenshot%202025-05-18%20at%2014.08.18.png)

Jika surat keluar merupakan surat balasan atau surat tindakan atas disposisi maka tampilannya akan seperti ini.

![Detail Surat Balasan](./ss/Screenshot%202025-05-18%20at%2014.15.35.png)

## Kategori Surat

Anda bisa mengelompokkan surat-surat dan pengelompokkan tersebut Anda buat di sini.

![Kategori Surat](./ss/Screenshot%202025-05-18%20at%2016.34.29.png)

Di halaman ini disediakan fitur [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) agar Anda mudah mengelola kategori surat Anda.

Anda dapat menambahkan kategori baru.

![Kategori Surat Baru](./ss/Screenshot%202025-05-18%20at%2016.35.39.png)

Mengedit kategori yang sudah ada.

![Edit Kategori Surat](./ss/Screenshot%202025-05-18%20at%2016.36.54.png)

Dan juga menghapus kategori surat yang sudah tidak relevan.

![Hapus Kategori Surat](./ss/Screenshot%202025-05-18%20at%2016.38.07.png)

Tersedia juga _bulk action_ untuk menghapus kategori surat.

![Bulk Action](./ss/Screenshot%202025-05-18%20at%2016.39.19.png)

Selain itu, untuk memudahkan pencarian data juga disediakan filter per kolom.

![Filter](./ss/Screenshot%202025-05-18%20at%2016.40.30.png)

## Pengguna

Halaman ini digunakan untuk mengelola pengguna aplikasi Anda.

![Pengguna](./ss/Screenshot%202025-05-18%20at%2016.42.52.png)

Di halaman ini disediakan fitur [CRUD](https://en.wikipedia.org/wiki/Create,_read,_update_and_delete) agar Anda mudah mengelola pengguna di aplikasi Anda.

Anda dapat menambahkan pengguna baru.

![Pengguna Baru](./ss/Screenshot%202025-05-18%20at%2016.43.15.png)

Kata sandi yang digunakan untuk masuk ke dalam aplikasi akan dikirim ke pengguna baru melalui email setelah akun pengguna baru dibuat.

Mengedit nama ataupun jabatan dari pengguna juga memungkinkan.

![Edit Pengguna](./ss/Screenshot%202025-05-18%20at%2016.43.41.png)

Jika pengguna sudah tidak aktif, maka akunnya juga bisa dihapus.

![Hapus Pengguna](./ss/Screenshot%202025-05-18%20at%2016.44.02.png)

Untuk memudahkan pencarian data juga disediakan filter per kolom.

![Filter](./ss/Screenshot%202025-05-18%20at%2016.44.35.png)

## Jabatan

Halaman ini digunakan untuk membuat jabatan/unit/bagian atau apapun Anda menyebutnya beserta hak akses aplikasi. Di halaman ini Anda dapat mengatur jabatan apa yang bisa mengakses fitur apa.

![Jabatan](./ss/Screenshot%202025-05-18%20at%2016.49.25.png)

Terdapat beberapa hak akses yang tersedia berdasarkan modulnya, yakni:
- **Pengguna**: `ViewUser`, `AddUser`, `EditUser`, `DeleteUser`
- **Jabatan**:  `ViewRole`, `AddRole`, `EditRole`, `DeleteRole`
- **Surat Masuk**: `ViewIncomingLetter`, `AddIncomingLetter`, `EditIncomingLetter`, `DeleteIncomingLetter`
- **Surat Keluar**: `ViewOutgoingLetter`, `AddOutgoingLetter`, `EditOutgoingLetter`, `DeleteOutgoingLetter`
- **Kategori Surat**: `ViewLetterCategory`, `AddLetterCategory`, `EditLetterCategory`, `DeleteLetterCategory`
- **Disposisi**: `ViewDisposition`, `AddDisposition`, `EditDisposition`, `DeleteDisposition`

Anda dapat menambahkan jabatan baru.

![Jabatan Baru](./ss/Screenshot%202025-05-18%20at%2016.49.41.png)

Mengedit jabatan yang ada.

![Edit Jabatan](./ss/Screenshot%202025-05-18%20at%2016.50.10.png)

Bahkan menghapusnya.

![Hapus Jabatan](./ss/Screenshot%202025-05-18%20at%2016.50.40.png)

## Pengaturan

Pengaturan dapat diakses melalui menu yang ada di pojok kiri bawah.

![Pengaturan](./ss/Screenshot%202025-05-18%20at%2016.55.08.png)

### Profil

Di halaman profil Anda dapat memperbarui nama, email, dan bahasa yang digunakan di aplikasi.

![Profile](./ss/Screenshot%202025-05-18%20at%2016.56.45.png)

Jika Anda mengganti bahasa, maka seluruh fitur di aplikasi akan menyesuaikan seperti contoh berikut apabila diganti ke bahasa Jepang.

![Dashboard Jepang](./ss/Screenshot%202025-05-18%20at%2016.57.55.png)

Di halaman ini juga Anda dapat menghapus akun namun **harap berhati-hati dengan fitur ini** karena data akan dihapus permanen.

![Hapus Akun](./ss/Screenshot%202025-05-18%20at%2017.00.02.png)

### Kata Sandi

Di halaman ini Anda dapat memperbarui kata sandi atau password.

![Kata Sandi](./ss/Screenshot%202025-05-18%20at%2017.00.55.png)

### Sesi

Di halaman ini Anda dapat melihat perangkat yang sedang menggunakan akun Anda dan di sini juga Anda dapat melakukan logout dari perangkat lain.

![Sesi](./ss/Screenshot%202025-05-18%20at%2017.01.04.png)

### Tampilan

Di halaman ini Anda dapat mengubah mode tampilan entah menggunakan mode terang, gelap, atau menyesuaikan sistem.

![Tampilan](./ss/Screenshot%202025-05-18%20at%2017.01.17.png)

![Tampilan](./ss/Screenshot%202025-05-18%20at%2017.01.38.png)