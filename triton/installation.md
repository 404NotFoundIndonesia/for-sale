### Daftar Isi

- [Docker](#docker)
    - [Persiapan](#persiapan)
    - [Compose](#compose)
- [Manual](#manual)
    - [Install Dependensi](#install-dependensi)
    - [Env](#env)
    - [Migration](#migration)
    - [Server Aplikasi](#server-aplikasi)
    - [Production](#server-aplikasi)
- [Login](#login)
- [Issue](#issue)

# Docker

Instalasi dengan Docker sekarang hanya cocok digunakan untuk `production` dan bukan untuk mode `development` karena isi project akan dicopy ke dalam container. Pastikan Anda sudah menginstall [Docker](https://docs.docker.com/desktop/setup/install/windows-install/).

## Persiapan

Buka file `.env.docker` dan sesuaikan isinya. Pastikan tidak ada yang dikosongkan. File ini akan digunakan sebagai sumber dari _environment variable_ di dalam container. Untuk dapat terintegrasi dengan AI, pastikan Anda mengisi variable `GEMINI_API_KEY`. Cara mendapatkan `key` Gemini silakan merujuk ke laman [AI Google for Developers](https://ai.google.dev/gemini-api/docs).

## Compose

Ketika pertama kali tentu saja kita harus build dulu imagenya, jalankan perintah berikut (hanya dijalankan satu kali karena untuk build)

```sh
docker compose up -f docker-compose.prod.yml -d --build
```

Untuk selanjutnya flag `--build` dapat dihilangkan, sehingga menjadi

```sh
docker compose up -f docker-compose.prod.yml -d
```

Anda cukup mengakses `http://localhost` agar dapat membuka aplikasinya. Untuk login bisa menggunakan [akun bawaan](#login).

Jika terdapat error silakan [laporkan](#issue).

# Manual

Pastikan Anda telah menginstal:
- [php8.4](https://www.php.net/downloads.php)
- [composer](https://getcomposer.org/download/)
- [mysql server](https://dev.mysql.com/downloads/mysql/8.0.html)
- [node v20](https://nodejs.org/en/download)

## Install Dependensi

Jalankan perintah berikut
```sh
composer install && npm install
```

Setelah berhasil dijalankan, pastikan ada folder bernama `vendor` dan `node_modules`. Jika tidak ada bisa dicoba lagi atau [laporkan](#issue).

## Env

Jalankan perintah berikut
```sh
cp .env.example .env && php artisan key:generate
```

Jika tidak ada error, buka file `.env` dan sesuaikan isinya terutama yang ditandai dengan `<Di SINI>` di bawah
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=triton
DB_USERNAME=<DI SINI>
DB_PASSWORD=<DI SINI>
GEMINI_API_KEY=<DI SINI>
```

Untuk dapat terintegrasi dengan AI, pastikan Anda mengisi variable `GEMINI_API_KEY`. Cara mendapatkan `key` Gemini silakan merujuk ke laman [AI Google for Developers](https://ai.google.dev/gemini-api/docs).

## Migration

Untuk memastikan `database` beserta skemanya ada, jalankan perintah berikut

```sh
php artisan migrate --seed
```

(opsional) jika Anda ingin memiliki [data dummy](https://en.wikipedia.org/wiki/Dummy_data) silakan jalankan perintah berikut

```sh
php artisan db:seed --class=DummySeeder
```

### Server Aplikasi

Siapkan tiga buah terminal atau CLI dan pada masing-masing terminal jalankan perintah berikut
```sh
php artisan serve # web server
```
```sh
php artisan queue:work # background job
```
```sh
npm run dev # build FE
```

Anda cukup mengakses `http://localhost:8000` agar dapat membuka aplikasinya. Untuk login bisa menggunakan [akun bawaan](#login).

Pastikan Anda tidak menghentikan proses ketiganya. 

### Production

Di live server atau production Anda tidak perlu menjalankan ketiga perintah tersebut. Sebagai gantinya bisa dilihat di tabel di bawah.

| Development | Production |
|------|-----------|
| `php artisan serve` | Gunakan web server seperti [nginx](https://nginx.org/) atau [apache](https://httpd.apache.org/). |
| `php artisan queue:work` | Gunakan `supervisor` |
| `npm run dev` | `npm run build` |


# Login

Silakan gunakan akun berikut untuk login.

- email: `iqbaleff214@gmail.com`
- password: `password`

# Issue

Jika Anda menemui `error` atau kendala, silakan laporkan di [Github Issue](https://github.com/404NotFoundIndonesia/for-sale/issues) atau kontak kami melalui email di [404nf.oa@gmail.com](mailto:404nf.oa@gmail.com).